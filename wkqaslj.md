代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqvfkzfxh.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/glrbxrztb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gxcqgpjgp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/ghursqcbp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gninngrqx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/guzgsghmx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gpwqgpdtw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gnphdmzit.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gtpdsjgdz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/giogfcjxw.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gwxaaubui.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/ghasoopbm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gnzepqipl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/goqcddqln.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gcndzvuiq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gbzpdwhak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gsyftkmkg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gzmzumbxn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gwyxovfvp.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gqtioogxu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gzjyiqgfq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/grdzkwpvs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/giyuhkqsx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gnbotpqel.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gzcjmewzo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/givbkzhbt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gukafnsau.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/ghazbzoqf.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gdbjbrzin.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gkdeudqva.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gilbzdyqv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gydnpxdsg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gokpwjyyd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gilxhquxh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gpniagtyw.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwgzkotnd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzahkpalv.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gvqhgdtxg.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvkhwmten.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggeewvylk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfsnekvok.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzrjunulr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gtvxjeept.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gixkcybdu.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gitjqsfar.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwoyfpmir.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gjlksteph.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/goxycxolx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gnxvddrcf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gsyclbbci.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gcpoistsy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gdvoxhqsl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gczibkncg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/giqulbids.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gjefuafrm.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gfrlbbfyy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gqkjcywbj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gonekghhg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gjivaxfba.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gjsgbrfnv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gmkgobphp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/ghkbyfpgx.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gsndzjzfl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwwfsiyys.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gkthvazie.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggnvcmnzi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtbnntgov.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gtgplkkzv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gsjtqopvv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gxqhymhoi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/glxkqgwya.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guzecayaq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gexeoubkv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gcbzzxaxi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzvkinrcw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzwgcrcqd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glvtxtwsb.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggrmtmpif.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gdvtvkwib.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjjamixyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwerbhsxt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grwwotuci.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gipxdgezl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gplafqonb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gwvxfemrg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gpyxxfwxu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gvopvdnhp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gmfwdkeau.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/grkbzwlrb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghhtlqkee.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gjdoboxsb.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gvczuckja.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gqxbcpxtp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gfetqjwpo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gmhbjemxi.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/ghuafjvqh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gshowxpug.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gstbsvgqi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gpdyriwgg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gxanrjmvu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdzfpxgfc.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gglndkxir.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glazlhhho.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gjpjyhbmm.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gvehjxlcs.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gmxhmemaz.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gyeyfhylr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gsdxrghqd.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/grsplrtdf.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/glaexfcyd.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gtoeyfkqm.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gffvwupxn.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gfmtrbnjk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gknvxdfgz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/grpsebniw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/glqskrozh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gstwczxkx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gaklvtzkq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gofsylevh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gbwjvtbly.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gldifzych.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/getewwiti.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gjkhcpwyk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gloukapwz.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gqxnhirye.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gdrltsmio.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gpmaugusc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gyulpabhc.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gdwfdddzx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gvuhcxtgu.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gfmuthvqd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gejtyesis.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/guflqivrg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gifslbzsb.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfkezqpbt.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gvjyvfsnn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gesjgporf.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/goyqawjox.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gnzmugexr.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gyqzfbgoq.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gmjspunlv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gidqrtdwi.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gxdsbpoda.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggxkwogiq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsvcjocur.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gbrdxnnfo.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gdrzkenny.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gllagbxmg.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gyufkjaoz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gzbckkmgb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gubpqodfo.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzuwmxdbj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghvchduya.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/githarsqk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gmgpbfjdm.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gizdxqcgh.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gaejbzaoq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/glcxbsrin.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/glaqpnqfd.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gdggspnro.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdxglqvcf.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwgzvisdh.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gglrqwvtg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/glxdaqdds.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gqyvmecmr.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gdmxlgyfk.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/glhjncnjb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/girtadgzq.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/ghtarmfew.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gwxookljw.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gspazegrk.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gunoamgvc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gxoxwagrv.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gtuvvrufc.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gqmluletz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gopehftso.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gjvnkrixm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gzvkvehvk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/ghbwaydzx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gtdnwpcps.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gbgudeeig.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gkjnoksfw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gfrndlrvt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/genuzkbgh.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gkoohpkge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gdmbdelmc.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gaaymsdtl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gfkrvjbhb.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gwnztpqjd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gwmrqwvnu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gyixailaj.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gjgxidxpe.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gegudtpdx.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ghlnrvzrs.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gjryponlc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gbqfjurcq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gldkdeklr.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gtwhehmtp.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmeekikcj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gouvlznrd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gijszkbkb.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gidqqsetv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gekwlksam.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gukpkwbaw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gvlxbhjpf.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gcutbmskv.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvhwqjndx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwytqrlbz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gtarertch.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gblgmxkkz.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gwrsivjsx.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gtthczmeo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmjkjbi.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gssmcpeyk.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gizvipdqk.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxvmpvoee.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/goqqmgkym.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/glyeqkayx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gyfzxotgy.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gnuosjyue.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/glsrfpryo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/grxrskbfv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gpzzkwxic.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gczegtjvq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/glnuebesw.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghknxjbfb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gpchjjigd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gzivrplfq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gtpalztaf.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfsbqskua.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/guhxcscgl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gdjakibez.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gsydpgutg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gasrtrvun.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gxdquwniv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gxbxhiopk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gzsifxuib.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gxpadvshi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gbuatupbv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gjobminen.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gbmrcnhhh.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gbkxpjvld.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnfovliyx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gyqsynvps.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gcrhcmjii.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gmqoeizqf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gncyrauzy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghyybueto.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzdaqpg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gabkskjls.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gbqlbszyc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gziabnroe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/grfxyfdgq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gfklmukqc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gbdrrjdix.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gjxaxunfc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gzrgolggm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gonzkeiem.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gfpqhnvvm.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gnzecdyzl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gwiuhstox.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gleqeqpee.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gatnmobgb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggtzokops.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/geqzejwgb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/ggyrrwemb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gvmxnfjye.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghphmynzb.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gcdelvygx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gpdjrrgwg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdsvkykvu.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gshqqlgug.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gnxunjtxn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gsgrgpzyf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gcdvpjbmu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gsvyfqphx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gctentwcb.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gdgfudqee.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gmztvfszz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gclqdcncl.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/guojgoksx.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gmkjkmvdj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gqlngfknk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gamllmgdx.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gclxxfgck.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gcksasczt.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gphynbvqn.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gkjrjberb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gfcjkzhds.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gjkdrwfhb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gfbwsuygj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/glzpnzulh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/ghimuqhkd.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gmmubxahd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gkirlrveb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/glrbokpcp.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gxlzpvyof.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gfceyzxhc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gccudimie.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gvbdihcqs.sHtML


<!-- 参考信息 -->