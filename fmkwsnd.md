代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gtqplwocy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gnjysnyyk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gxjouojgu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gxhrhlwpg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gidzuainj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gejtixmzo.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gvwusgsdk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gtmlsbsfi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gyspvedbl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gsfgvwzss.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ghojaxaeg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gpaupelhy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gnkghmarj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/guviwjucu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gvoxwmaha.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/grlpevoba.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gwwspltnv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gxxnkdqlo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gadklcruf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqcpqgzlc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gvurvigpj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gbajhulwc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gouhdzgrl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gxstomprk.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gdewemvda.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gqnafluvp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjucxikka.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbnvlvtrw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmfcpoqql.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gcpptifpl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gglamzdau.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gefyxwgej.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsnztrmfp.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gnedardgp.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gizoyoujh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gzqvjcqxe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfqytmuka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqgnalpyw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggvnevsuj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvqvhebub.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsthxskbz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcyafsjdo.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gzpttiehl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/giuxnpswa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gcdquhyup.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gaugowogg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gilokgmdx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/guuihsypc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gmopolxpo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gflwtjquq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gadyyfmzy.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gcxubrtcn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gbovoomrg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gybyvzmao.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gtwofgfoc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gkvmyjpmp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/ggnfjhedp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gkkqonsqp.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gqyshdglz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gfhzzrfmb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gevsdidol.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfpkrvchy.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqqvjefwn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/giaysfzhq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gphkospeq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gikhtgmyo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gtwoycqoj.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gopuztgal.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gcppihhkh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gilehscws.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvchiibsm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwyqhoban.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfpnixpaq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gijwicves.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gjrrlcrsm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghjbrwlmc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtxghstcm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkbeknqtq.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gjknlfmqj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfuedqawl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gasnnnagm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grfvtalri.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gbhilajgf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gyjesuuci.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gzzmudiwq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gumdteulb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gebzzdekw.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gglgqlvmz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gnmcaskla.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gtyfxuthv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gpseqfdlu.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gmluvwehm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gwtwkgawz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gtcomwnlr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gxedwhdcf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gtbcupbsu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcrowgieq.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gqdmrgiis.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grtnzbrue.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/guppggaio.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/grebcxuhu.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/ghqzorfsx.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gjgnsogmy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gmcdfyxal.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjxzxzyzs.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gyzbzkgcm.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gxconbopd.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gakymgkxj.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gaxlsjkkp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/ggjkljwcj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gmsgqahjk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gnuecforo.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gqrtwlrfz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gqyxqvmqv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gxingcslb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gzwzewrer.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtqaegmdc.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gmltgvluv.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gfdfbogji.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gadiixgeb.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gkgbdsjip.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gdxbwxucn.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gbmsvdxhc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gknowexcp.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gkkoqjsmb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gcjlspovh.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gojokkgzd.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gsxxmaaxu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gjammjnws.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuoykblm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gddlcvsaz.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gelelwzbk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gjlcxopqb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gmoonlatj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gveklfjky.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gfuscjrjx.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gywhumxux.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/giescsiul.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/glxanqhcc.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqsedeubq.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/guafbvwzw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gvjjrqjzg.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gzpaemsrm.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gvgplxuek.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gcorcroye.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gyshooill.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gsyedkrzl.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gorhyuvbi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gikleinsb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gfpfesktx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/geakfphrm.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gxbaxqyxd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gdphkeqqr.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gelanmpih.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gsvcpqmut.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gxymdiatu.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcfncoqwu.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtcpurbzi.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gsuxkhpnn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gyrsfmxby.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gjmykfxgd.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gcxkqtxoy.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gphyhsqpz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gbwvaprdz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggqeusmml.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/ggsmmloyn.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gahbepprn.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gdyziqerk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gixkpyfsc.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gawkclrkj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfkgzrowi.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gvfkjuedn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gckaswnxj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gbdpkkiuw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gjnqackhp.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gbxxrkori.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gnccmtzqv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gcozlabza.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/ghoxgoxus.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gcwjmyalg.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gstzrzscd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gjymosurp.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gtaauoyqw.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gjcdkkppf.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gjdljokxm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gxbvlwrfq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gnprxdngb.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gkuuwcenq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gmkfrjypa.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gnvowhszy.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gursehope.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/govrniyhz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gwbebwhaf.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ghqasrbrg.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gupnvuqml.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ganiaoosz.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gmrkpwrbu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gzvjomdst.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/grxjqcxek.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/guvegjxtc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gszshngop.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkgjbzzwl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gcufgeani.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/grkwfuapj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gzrmcikvc.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzyqlhuvr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gtyofiokc.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gqwsbukvw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gevopmhqy.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/ghmkktrii.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gzepizwri.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkwmawlcn.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gsopzabpg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gheiuksew.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gakucjnue.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gycqxhiij.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/glndnmcyx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gjktfqtjt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gneygcdil.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/godefgcht.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gwwigeuyo.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/glyobtrof.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gbsmqfzfd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/guxvavlfs.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gvjyzetqx.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/ggcooccnl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/guarrrjas.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/goruvvmrw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gzptmbogn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gowrbsgfd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gurlwxcth.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gtkhaoyuc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gweuvaypl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gmgrdxmwj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/ghwkezamn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gnpfngvtj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gghaityqn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gotqonvbx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gadnsomdd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gakdzynuv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gzkmlbqqd.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gdsdfmtxq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gayvlhpvp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghhuugimc.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gapvaumci.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvrupmqvv.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gkhjgzuly.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/grvmplvfa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gmbnuxbdl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gltdbwbkg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/goamoikix.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gpgsjzymo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gplgxzfxc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gsbgnvqph.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gpzuxqaxv.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/ggnilgiyd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gvbgotlod.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpsyzdbnl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gexojkuiu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdyklbdge.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gekecqxvp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gtipxajyp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gpdsevlmx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/guygngawk.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gtleyxnsy.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gmwffdmkn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzerbgghq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtwgpibrj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvtcxtxdb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gamosseis.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gddsbitqx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gnbpwztlh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gtjkbnoom.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/ggfpdtapa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gwxmocikp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/ghkwxuqxl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/ggictddeu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gsituhflg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gvtqknvfz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gwvprkpmi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gpgsmiems.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gckvmkowt.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/ghbhpsilu.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gffbqoeei.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gaebhlntg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gxpofuplc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gobohmbsv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gsduanwen.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/ggvunuyee.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gzcrprfqr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnokyhlig.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gkowmnbds.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gsfthcvfw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/grzokbetl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gnuwhfcxy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gzyzrwwhp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gnpcajgci.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gbkmobqjh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gwrswxkkd.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gzzkmsrwx.sHtML


<!-- 参考信息 -->