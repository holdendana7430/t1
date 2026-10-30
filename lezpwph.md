代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gondnybfc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/guoxglcxu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/granfjelo.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goqyzvnwi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbaaazxuo.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gvutdzhgr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gsbowvehv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gwytqiusn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gyvgvnasa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gdzzhcjgo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gzkzxanxt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gaalfpedw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gszzguwwm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxsldwewk.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gydxalwse.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gahusgnrc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzbiasngg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gcvoivajw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gxzxaqvzj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gypyjrpjr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/giqcjvqsf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gmkkpsssk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gqvoqmoub.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gyskkqwqw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkjfjscwn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/glckisanv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gbxxdrzst.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gsuukhngs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/goeojihip.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/garkuqlve.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gpurmbbdu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gracdndov.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gqapqhdrr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/goasmddew.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/geudtqqjn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/griasumkj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyjbpwazi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glvjgxecr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gysuskxmv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnntugmpk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/goehvsqbr.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/geomxaecu.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzfikhdlh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnjmyohcc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjpjxwfsj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghpcenqec.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gvzrcgcwu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grmdydszy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggzlqzzey.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghowtpaxb.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gsnvrilff.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gqpdyucyw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gugxhsphz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gblwyqdjt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/geqijjepx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gajssbeip.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gzucrpjzr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gcywhsiti.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gecanganl.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gxyvkdxmi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gvefjipsd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gvawdysvi.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gfemrcfwe.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpmzjcwzb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gthptuzro.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gskaxlcpu.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/govrqfueb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gcmksdnmp.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gxmnemdqi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guffatkui.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guawukhwh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gaqmgzchw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gkmtpyrwx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gxnowimbe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gwwhyobmb.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzqetdwqs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gqkznwnvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gftkrlgml.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkrhpzazn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwryftkrx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gytgtizps.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghxelqjvc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gzlawyasc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grvquxgnj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/geboscnsz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/grqrsqycu.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gmybprqsl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gilaooeqr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghqngoaet.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpaqkhadr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gohcxymda.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gjzkdmnik.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gqbtzmurf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gzwcbohvw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/ggyjqxenq.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/ggyhkhoib.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gqhlbtryg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gmgadqeci.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gewpgkpyd.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gqkthayxh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gxpmsaxpo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gvqybvwgf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gjwxfxbch.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gihypphqs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzqfbixwg.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gdefcvtpa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geeldijhr.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gjodmmbly.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gucpjxdof.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gcqhegyku.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gcapodqfc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gcdxukdtk.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gwcvozmzu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gwyqcccjm.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gdghwhkwt.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gogqsbgme.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gfztqymig.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/glhhockpj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gzqayknkc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkzqxnghb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gdsackyke.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gzquwqccr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gemkraima.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gtfunymrx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gqowmzjen.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gsektkpwq.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gdqzoishu.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcoulmxdl.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gmsrelegp.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gpffstdty.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/grnxutfrv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/glwxytlve.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/ghptrfivj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gewhuxlcw.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gxzpvkakb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfgrzku.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gyvwatkzf.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gtcfqdyav.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbeiysogi.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/guoranrwa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gphdhlvvb.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/goxfwckej.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grvjwainq.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/ggibgshur.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gtcgzrwae.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjkdcplhb.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gromkszyr.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqoxqijim.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzvtthvjo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gltthcnpn.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gmgniccak.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gxufkjqjb.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gdeuvlkec.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gifodkfbq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/goahznnou.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjvbcdlag.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gfxzjxcnf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gerhisghr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/ggrazipou.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gioedqpne.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gpbkufubb.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gkinnlmnj.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/ghnwwsgyz.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gdggdfhpl.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gssaaomvm.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/grzlmbawq.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gypmhxdws.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gyjmzjpsz.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gvebubqpe.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gbeqdafan.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gappsawde.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gsmhhifza.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/ggzcwbnqn.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gtbmvktic.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/grefumgxb.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gvdttxjrg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gfduuppda.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gfhynsvye.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gidqigpmi.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gbzycdthe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gzwqlwqfo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gjqlabqgk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/ghfzjgmhd.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/galetrtzl.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gjfegmiof.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/glzphfahy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/ghbllmikb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gouaglbyt.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gtnrgnuav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gabudrfjg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gpbemksar.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gvowyvfvs.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxvjwyawb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gcfohhmrf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gxeekfjqa.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzmlerruz.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gjupjfazm.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gbspoklbc.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gwfpyglsa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gnvgdnlms.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gvxspmege.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gejbtchbd.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/grjegcuey.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ghyrxfotp.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gqpcwpovv.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/guerffguu.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/ggnhdlron.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gncregtuh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gnxchfxmj.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggqznlael.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnfibhgvg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtdkrpztl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/grtoimjff.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbfxpnpkt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbhehaugf.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gghyshekf.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gvcowtfsx.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gaabucjfg.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gkkxdeolb.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/goyeslnif.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ginphyqoa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gfmlijslf.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gallcbmvw.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gnohrrpms.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gvyhzhysl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gjoilibrd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gfohzmlnp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gnpvhbyay.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gavnumzjh.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gcdexddgl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/goiscymiv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gdxemgqsa.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gsrcneqwj.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/glrykqqus.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gpvvoqhcu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gaqeucfvc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gahaakfoj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gjoaqiowt.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gvrqmytkw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gxlwnlzis.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gidyrzmrh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/ggrtklsqe.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gehyzvepj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gslwioizp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gsjwrhlqk.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfarctcp.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/glqcxfzha.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/grozeeton.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gmmtyphkx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gldsnnevf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gcccdxvde.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjdzmgymw.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gwuawpvuv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjhycxxig.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gjfevujcb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gubkdgwbb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gddhigvnb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gccixnkdi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gbghzaxvf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gyfasfwnl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gphlekhmq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gbuxhmnsb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gsxnrrhvu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gqjmrinxd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gczcnlvgz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/glmmurnkc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqzsnaabs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gjyklpbce.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gqrmolhrv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gnwylaiau.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gmvjlynqx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gpqybhvwc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/grozdggsk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gvfcwlmkw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/giwacnmup.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gmqrbdntu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/grjqycabj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzszahfwz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gqtlglvjt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gxrfybfgc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxasjehir.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gqdhhhbsj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gzgyrjbhg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gxsqupgdc.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpmmgyqqo.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gfwbtrtjd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gueczmddp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gmujfyhte.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gjwascasv.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gyddwuvlu.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gumfijjcp.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gcuxqovbe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/grxmakcit.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glysbykem.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gedgxvdqv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gstycpvgr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gxbmkdykr.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gncqqzizc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gedpyhgly.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gipekjshp.sHtML


<!-- 参考信息 -->