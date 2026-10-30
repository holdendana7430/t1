代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gavxqqnxf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gbmedhocp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gzzijxzgh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gxskmhtmg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gqjprpgqq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gdirleyof.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gjbdgfize.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/groravnuo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/ggzmqdzgq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gehrhszmb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gzxjwewea.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/grapewaec.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gcsbzzswl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gnkwbhdqh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gsqampkym.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdfbtfs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/guhcgmxtw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gppylcoja.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gieglqgak.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gxnmwbhcz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/goswpffoa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gylnjncir.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gokvwlxwo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gideqlufz.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gdihgmwmh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gfiwzlvao.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwvddximb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxjyppzpi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/giqbsjhwh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbrikbayk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gkfdososo.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdpmfwutm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfhajwohm.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gnqbbxbne.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvrquygbs.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/giybzviyn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnpuspaky.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggemgukfd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gzllwakih.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghstroctz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzcobpbty.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqibwxsle.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gaxvidqtf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gqpdimbdn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gavgzfgwa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gfiilzner.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gbrbiindp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/grrouzoke.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gysrqcjhv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gxenwlbop.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/grmwhovav.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gmlqnhdmh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gwywvcdlb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gypptfgff.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzodbwlnd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gijdetaqk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gusvyppif.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gowdebtew.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gtlszhulc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gxiskwbrn.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gzssnhlcx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gahpfimgd.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxpvqwqdg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwsbxxafv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gljbkfjnf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gzeqgwaar.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/ggnkvvljy.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqdlcliyn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gzcenclaf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/goxkeoynx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gglpxrzex.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvmxrpvhp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guiragnnu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghoikosth.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gnshniahe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gckitrhru.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpdmhmcdg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnrpqsnds.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gzwmiytck.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gaxslgcjn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghcvzzbzn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gnlvbzxuu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwwhkyorr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gdooukehk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gzparszau.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/grvjoxhpb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gzjbraock.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/groyosfuc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gcsjnqkjw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/giuoxddjb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/ggmkuudtn.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gtmpitirq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gydknhtuv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gklwyiaql.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gpxorypws.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gpvmercea.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxnesjcjh.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gnasbofhg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grzjrlduv.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/ggpljdefq.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gewygfcoh.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gezbzvmhz.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/greicgyvn.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gcwkhsrgo.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gavssmepr.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gxjnshary.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gawwbycnv.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gcjevmxff.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gryynqrej.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gghbdbnas.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gylsrmkgm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gfvgleecm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gukqmgkhb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gdurfrsac.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gcruyeipe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gqdhlxdwb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gnfrljaek.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gwbnvqinx.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gcaxvvcbv.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gpwnzvpyw.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gkjxobgjm.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gpsjhcoem.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gesgxrokc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gyxhdlurz.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/ggplxqncl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gqljlwixu.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gyjhlobiq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gwdgximtk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gplwvdtsl.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkgpviqda.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gelzaugbc.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggbxwujyc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkhkuoqgq.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ggmvixpfz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gpyflzjoc.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gvrrxxqua.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/goyetdfmm.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gufeeftoo.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gqdugyimv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjekbhfk.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gsjxgqtox.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/ggnlkgxab.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gfkrzutjl.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gkgajhwqi.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gukkpolcn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/ghwroaytc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwxmbriiz.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtsrtpcot.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gicqyyxts.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gemcyolzz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwwzpvemn.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gjkcbdzky.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gkxrpaobr.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gndlmifwv.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gbqjjexkz.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gbbadoqjk.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjkgikcuq.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdqrseijm.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gptlijlmo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gvxiyhbsh.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/githmuwyt.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gtlbhaojb.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gnpdjlczm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/galhxxyjl.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gltiftlvf.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfhbpvfla.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gyiszqqtx.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/giwkjfvsx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gwphvggpd.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gzhmebzua.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gtxmiaxwz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/grtebexjb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gwpvnpasx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gmtgdrivb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/grrmyspdl.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/ggvyadsky.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/govpiefte.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gocudwplf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/glrkbmqzz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gsibhxzcj.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gcjrzdjiy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gmdhnuczi.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gcikngfdf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gryucaaic.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/glgpqrurv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gmxsekcri.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gfatcxrxe.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gvqpfusbs.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gkoqyqjsd.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gfpmxmswv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gxtbgdrjf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/guqncstno.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ghyworhsg.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gnppkccis.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/glxfpmnqy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfipbfhlj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gtrvgazja.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gpxrepuwb.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/glmcbacop.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkzzsxa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gqqfbegfc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gesganvaf.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gowylfkej.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbmkelhex.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gogdacppo.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gzmnobqkl.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/glewxsaer.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/ghwovbvlz.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gxvhmnyfu.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gssgikieu.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gaxmpjzip.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gqceuhilp.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjhapqmzx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gducqdpjl.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gsyfymeba.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gpnkpmuip.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gmivttfzx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gxifarief.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gupfzyodm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/goipswlsw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gzizoxqlj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqcdcwoye.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ghxfkcypy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gnqdcrrzy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gvmetwgym.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/ggvqtsdgn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/grykbttpw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gqwdvfyog.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gzujorajf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gmkwgkvxx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gtsulqazu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gkyfxfsqr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gzbiideba.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gstecriyg.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gyiyeiojn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gyyiqtckh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gjtqzdwln.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gzjzgrvvy.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/glnvojelq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gphmqbwps.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gnelhissm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gcoetrqyi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/glijmnqmh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gswnaebbv.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/ggwsfqujo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtjxdwwbh.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gjrgntghj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/guwzsqljs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gicurnpnx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/guojcvclv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ghrnlgqnw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/ggdzqzasl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gwudzypxb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/guxbfiwmq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gkmhurigj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gxiasrvuk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/ghbqvzgdx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcaloajuk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gvienitrz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gaoevhbiy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glouhjcnr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gtzuvvydt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/glcnrscyh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/glwngjnba.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gyrzxsoso.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gbxxnzrtg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gyqgimith.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gpbrvydpr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gzcawcgba.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gprlavmoh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gqwkfeotf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/ggqhyynog.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gurqbrulh.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gtyzvyisy.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gxscafcyx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gfmohtkau.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gqecgmlnd.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gzjhvtaar.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrckhrx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gejoruujp.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gnjnwpgvn.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/glldmeqki.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/glixxludg.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gyvhkrumy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gtlmqxthg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gslyhxcvw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gsqvgspsw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwwnmhkho.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gopovmrtx.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gnmqujwft.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gfjhxtjxy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gkounbuek.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gjwcttxtb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/ggdtjdjfy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gwexhdnsk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gxpskolnw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gdfcwztcu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gmrhxejzt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gozjlixsb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gvbxczlxq.sHtML


<!-- 参考信息 -->