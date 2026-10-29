代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gpbugfcvt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gyegyporz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfulifoqi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gqqrnugxv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gusfuzzqc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gctpnphww.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gpexzvjey.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gajnfsejp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gtadhbrmd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gbsxhmifx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gilflgisi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gohjixuvs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gtzztjeof.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gwcfrtwyh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gpuleppjg.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gckubrbnt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gnovhuayg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gzcxbdmmi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gbhfapcez.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gbzsfkdop.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gkntqunhw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gbwnasksj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gcsffxdak.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gbrsbyqpm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gjqtpilqg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gkynjymiy.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gldfvjctg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggprxquvb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggjanjxsc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glxlwofky.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gswlwnakf.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvqrjjrdf.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfiwvadca.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbypzzpje.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdgkxinak.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpxworokn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsnmyqgmb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqekymvee.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvwdefflz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwaoduygz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gftoicwcc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/givsrpqth.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gxmrssnak.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gpczmlpuk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gqajsikhr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gsyretnir.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gevyjedmf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/glkaupzxk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gpahkecfh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gbbzjaoza.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gslvmeeef.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gbomiphpa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gpyonyifo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/glumhpffo.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gcqroyoom.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gfwsjcmez.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gplzimdga.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnthlmnym.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/govxyxxwc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gsbppoibg.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gbpbuqiuw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyuulmvnr.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gsfeochyk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gzemnnhne.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gxhfqeygu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ghmqzfutz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gqonvwyfk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcapciejb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/giydxotzk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gfttnclvh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gacrjulbg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzztxjevj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwametfpr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gafpruxbh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gpubhmxwg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpgzjfxve.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gstnkvkcq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbohgqgte.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gowlhdnum.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/glxpagwaa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/ggucnncqe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gfxsskheu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gzchzehki.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gbxljytae.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gbdllaqbi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmamwuejt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gokabxckw.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gmfzvehym.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gieruehtp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/grxbvayko.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gxcuvdajh.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gzlyozfwu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gddpqneyc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gvaiplxeh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/glphqmzxd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gtnulgqcq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtvrzavcq.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gropdumxn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmbjgihxm.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gpufqrbwm.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gsgwhxotj.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/ggvrgqqsm.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/glfqfoaam.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gttaryosw.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gaifobhpo.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gxihlaxer.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gwnxjqunl.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gxdmbhvgy.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gbukzjtyx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/ghllllinh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gsmieoeuc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gyzmcolkf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvawmcpqw.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gaevusmsx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/ggtchgppo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/ghvqcklba.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gdbtgvtaz.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gentqdend.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/geqmuyugu.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/guojqmmal.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvkcqmrpz.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gzykldlkm.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gathdxkld.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gwpvhpypa.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gfvdninpo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/grryqfhhj.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gdxkgrvps.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/ggyefhtxf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gtxekelzw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gazekoumf.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glgekvhzr.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gzvjhtomg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gspotwqaw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/guvvgyaku.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gqxmctqzj.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gxlfumpdf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gzrrqbptx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gdtsnfeoz.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gunkwethe.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/geqxberlj.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdcdxmkgk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gmjqcsvip.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gncbqfofi.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gfhwbafoe.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/giydhcqqh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gebmpjuqn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gicobkmem.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gpwzrnekv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ghdhhngrb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gajndkpkv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gkgkxgvsx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/grpmvponq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gphntwuls.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gziqbcnow.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gtwbpnymb.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmksjfyif.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkszikoij.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ginzjsako.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/glnaokwlp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gdodulicw.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gekkjyeyv.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gzvllyhor.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gofcyuadf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gyltnsvop.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gxogjmkro.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gcepbflcl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/geclooeyw.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gsuhlmuty.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gotefgqwd.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/ghqamhjfq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvjhtvguz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gwzsubves.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gmozlffae.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gloyenjmk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gfbbjugej.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/grbvobngk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gjmathwwc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gqwywomen.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/geyhlstpx.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gosblenhl.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gscdtavei.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/grbmdfrsv.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghqgxxvva.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/guilkibxk.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gapgweleq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gtjlbfhom.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/glzjsvwju.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gaafhhkkw.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gejttutvx.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gfxnttomv.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gnadhwgis.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxzvqkpjs.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ghpcodyuz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpuimkfgz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggqcxtijc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbtzaagcd.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gdoasctmg.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ggkgkmavm.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gtkxsoory.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gnetgiqei.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gvurdibjo.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gveehqrso.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gqsheoodj.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gzytaursc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ghaanemkj.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gwlkbasyu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gdnmmouul.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gscllbdfm.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gajdcppuq.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gjsqrweoq.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gmgnmtbhz.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfbsrrvbl.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gqglvcucf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gaeviyjzm.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gbdardghu.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/guivjpkmx.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gwhfyqkbr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/ggsvftqom.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/ggzoocams.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/glemzpoiw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gfjezrqzr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gpvheszba.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gisrjjzjy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gwrxzptlv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/geapnffry.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/ghtmhinyo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/guggvpelb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gvgnnuzky.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ggoyyueyc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gxwhgxlke.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/guilxuknq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gevkvbbil.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gcueippvi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/geelcowhp.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gqajvthol.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gaqcksgqo.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gzwcvnmri.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gzunqxuec.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gdwddsgbp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gbrgcwufp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gsvxogqnb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gejlxgeam.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gutdxdcwc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmeaiulds.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gkbserkeb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqbpolqvh.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gljbvluuv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gibivazqa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gihjudnar.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gtvfgpufb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gsgeysxmi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/giyzlhxwz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gvpchbsee.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gbdatqtwc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gtrskmtsi.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gayylflwl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gagqwymum.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gbzogmswo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdtrtuifp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grvjzhsuw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gtihskfat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gkbzrdsks.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gzhiwtwmh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gqwvdnjwz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gurirrufo.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gyxvxhkdu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gvpwyxnya.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/guanvuanp.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gioylmdqx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gdodoxkvl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gogbjhksr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gyzfwxulb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/geniwblhl.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gmslehxzy.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gnbbgrggr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/grzlynliq.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gwdqajqmq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjhpgpwxv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/geyxqnasd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gbauncibo.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gcetmfjgj.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gjgqkhndp.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gbyxmizry.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gthjnumkq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gzerhocxy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gppoblbkn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gksybzroh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gklnnjffw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/grwfzolux.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gchuqvuim.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gqywrclob.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/ghgdjvxqm.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gafyxgouo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gvjgojgcc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gueohibxm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gwozstlie.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gmbfsqiep.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gsxtlavcp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gjjzgfegu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gchbdjakw.sHtML


<!-- 参考信息 -->