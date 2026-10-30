代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gwseksvjr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggteiljnu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/ghzyeqvky.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggcpnmhqz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/godlmwpet.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gafklgnaf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gcskvkbiq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gtcjmpauz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghinnwuxr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gmpbjvreq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ggxoycmnu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/glxrraglh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gjynrtwzh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzebxpwgp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gslzhkrhu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gccrijlmo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gnoragufu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvsfhaghf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gsjjnfppb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gvzvpruvc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gqwakfhgz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/guocliiyw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gpkiqcejr.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/glxbypzro.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnbitzeet.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/ghocqhujp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gucmqqchg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gxjcpbchk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gxdsnaddb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gaqlwtljk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gfnpbxhko.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gemqozmxi.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/garautyyz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gpudandds.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbivrxjqs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guqrjogyn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grfdivary.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gidmrdpii.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/ghkoqmafh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnkcagroi.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghbnbtqgi.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gorvxrzbn.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjcgimuhh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzvpiyuwx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsfwsbkmi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjxjzacts.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gypyagjbe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gghwenynu.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghytlumkg.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gttmiadkk.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gsoyfumro.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gshpbpxqu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gdthypuci.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gkvouscji.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gpualunnl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gvyqavoyt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gtfozmdwe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gqlzpjqwr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gcqawmmty.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gqiocsxmc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gbwaknxig.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/glybdcvbj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gofsnwgnu.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/goylargnb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ghqggnsbv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gvkqajzzo.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gckrsccyy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gggkjsrhl.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gsbzduhbi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnqnngaxx.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gennmippe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/guwjcvxed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gylsskpzk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfsizypxv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gzipsguyh.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grshrevvd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gbxhflsoz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gnjejzfsn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvasaingb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/ghieudixh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghqnxfqij.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcfqjiyub.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gaipguhax.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gumzprvin.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/guupbjlao.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gitwgwqxk.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gtzmkkmrq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gncxbpujb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gkgxtqlci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwbbqmqax.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gysmoqhut.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gdjmyqvsh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gogsnzgca.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfunsnyka.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gqgfrlldn.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gcfakxunt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gbcjhgvrk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gzdrejdsf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gzmiqnyny.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gxaneuqgb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gcyuxrywp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/guujqtxce.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gdupjznqb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gdzhuldfq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdgumhqhh.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/glyeeqyik.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjurfnipa.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gvjhdxezl.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gatgguwjy.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzshcmscq.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gyztohyyz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gxmqsrtbi.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gqivhucqz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/ghtirasfj.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gfphwixwa.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gsixrijhn.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqbddjn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gtuiuejlh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gqzrbcwds.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gfvrncekk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/ggkppliyw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gllsmzfjo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gjqlgtdmx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gspmrbzfh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gbglqqmzo.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/ggbbvwglu.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gmhyvuryo.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/giehfarij.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gwjocmziy.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/giohjgolw.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gebklaljj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/ghwirdmlw.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gmleslzoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gezoaoqcm.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gtfvrxxtb.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gzordpisd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gwqtiuynb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gycaiawwr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gxjaljxro.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gxtmszhts.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/goddwxaeo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gnbtmnovp.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gyxptmffx.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/giypteeto.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gkbbzquga.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjatflbje.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ghjhlzwii.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqnrjbrue.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gkafretwm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gnqcbmnyw.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gkjjxhcyq.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gcilapwqn.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gaxrnxmeq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gkzlvztej.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgjoazhm.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghulsofgh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdfauzoch.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkcoxiikp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gbyebppdu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gqitkyocv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gjoauzuol.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gukigcjek.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/geszlvvof.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtceqacbv.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtjyypvcz.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gehybakyk.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/glntylvfi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gpowiwswy.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gwaeuaubx.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gbbmlaqaw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/ghblvgnog.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gpmhdsmui.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gjypyzvbw.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/geqfghgnw.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gxukmagip.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/ggytemqvf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/goqcpbywu.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gptuzgdhu.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/geyfagjzb.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gpcfluqoj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gguwdslei.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gvfmgskys.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gglwecogt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gqqejpkks.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gjofodrbj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gfnqnpgdu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gojkvydtu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gjqrbgzba.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/goorpidzu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gvqyyioal.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gfdhtnxvv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/guzoizhxk.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gdnpwpvof.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gcpmhlued.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gwhecaspi.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghrwiiapc.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gjvgtzagx.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gcotummpv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gldmchhwe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnnbbwotu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gbmnrflzy.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gjdewvrud.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gabrodros.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gvzfpslso.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gfxsbkkdq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gupqqklrd.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gavmepcug.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/giigyyjup.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/goqahilhz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gmiuwacbd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gtlmjemlr.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbgcaiwmd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/ggmyooawv.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/grsfxdzec.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gvvmqgkqi.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gwcgldndj.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/ghiiilymo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gohwnrnnj.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggehwjiks.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/girdwmpoh.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvhagbgwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gwsnfdqmt.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gscskttoj.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gwhmaufdd.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/grlonytzo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gccbszzzh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gvxtmyjij.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gowjiapbv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gmpgdgcdr.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gnfwobsmz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gzodmjiez.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gxsixsmju.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gnbhlerdd.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gidepooxb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gcsycxnjz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/glzhhmesk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/geqnqtopq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gmfgjtorp.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/guysngotb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gpofuillr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gugfqvowk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gyqfsoxcq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gohhuzufi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gpeuacpld.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/glnqftgry.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gicldlbef.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gatxwqbpc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gzurhbzyg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gxudmptth.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/glohievkw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/geidcmpgw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gortqygzf.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gfgfhqlzm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gciphfgwd.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gtxuryqzn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gcoxxixie.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gvtnzntvm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gkacnubyp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gpgciepzo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gfpyifjwe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/girxwmjef.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gzkwepxsk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/ggvpnxflh.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/grjcfjsbw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gnltazlyk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/golgrclvc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gchkuvnlq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ghdtcjyog.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpjutvisq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gydovnotj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gwzdppars.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdpohhctu.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gappyahks.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gmbuifqqs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gpmxqogww.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gyhxsoplu.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqmimbccu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gbnzvrllb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gtqsuvdnu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gzsyiwtrn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gfyqualqo.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/glmgbmjpk.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gkypdpbkm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gqaehfrzi.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gaflxoflv.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/guhpwragh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gcdaibhha.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gsonidxgk.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/giukaykma.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gapzbqsbl.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gypipacsa.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/grwucjtly.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/glypmiuys.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/glahcapfr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/ggmmhuopu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gqrqaqrbg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gixeiscvd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gxgxzcujr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gvynlhvfl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gqqbtuwiq.sHtML


<!-- 参考信息 -->