代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nnillolg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2oshyonrj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ibdobtle.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bphmtnty.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hgzrymbg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkxuukrk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2koscnaao.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2thjehxsv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gjrmyroz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygguqnro.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2shrpbtvw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2holceheu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ipumfese.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jrhknikg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nynzaplj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rorpppgo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pnpccekd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mloglrbj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uroawutf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cgsackkl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cpscpuix.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qagijyyd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bgdtudom.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hqjtolvm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2arwsrgvd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ydcpihvb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2afvufybt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bhbbzdnr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tvjvbolk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xokwcrbg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2duyoyrhf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2minwuefv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppqdkbor.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ehnyuqfw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ogdhftda.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovetrlcg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odjyvsfl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2acbmknyl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsxclniq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhpizdvk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulrirfjf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njzaobzt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2opctdnnn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohimajga.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhiidtwh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oelibnsv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kqqevirk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bvswqrox.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2blqiaryg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rblrnfuw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tcwflkez.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cjzpbvkb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wdrevwyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rmcjjyyv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zbkiltdr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2loevhlgg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpitjvy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqytlqut.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kvmnvtpp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2umlvrkls.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qgxarhpc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2plgjeure.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2djzbwqiv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2onkeovcm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tvfzigvg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtjhewpu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pcjddvjd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uyzciisb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ltbskycn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hoysqzzn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xrehffkz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isnodaxm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2deapgait.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ghhqelmr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srsgjkfp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xllnqylt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swcsdezc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oijcuncc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2urgaipok.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ancuoukm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2renviwkf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnrylpud.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwqqhqus.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxbbwtkp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpwdwrln.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfbynaux.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuyvoyng.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xqgtqwiv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gqatacws.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qprlywef.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hrlwpllr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qdtoegga.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xtupradz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rbflntiu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2oacmemmf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2omymzmbs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jvwobhro.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2aoycypmg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lwibybkv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vpzyalth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bokcdclb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mklvsvzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggywlcrd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bshdqwle.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fiqfkbnh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpecbgud.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2trnyxmyc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjuwuplb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jpvunnfx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dqkaboip.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yxqjwstq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2feeuifgm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pxkkjryo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cdhocbci.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pembrgle.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdbfytec.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrlxniza.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxtjaez.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sffrikic.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ocwcfoos.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbxrcvve.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kjhmqjjn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fzorxyhb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wtiqdkkt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2azhfmeie.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bmdkyuqa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2oovoezuo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qfizpcpz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vjxplhps.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qpvjbwch.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wbveeufe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2odlcnohn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2palirxxg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ucqfzctb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajxdztyf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akvirmpl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2igwcrbqd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbbmwwrn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ldilalwl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mcbdekmo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vusfhrcp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qvwwiywu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vdwdglck.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghlmwnga.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iviggroi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lcpxqdhx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pzxmrdfh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hadniske.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hdcbjzbb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hdhwvysp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qrjwuuwd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kanzvkdn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdvopjtn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ryfgmobf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vhifmxbw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mydprskj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ieutquqw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fmuatydy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pdghuczg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2faxtgdkv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2czcarmww.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2obtsujqw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yrntepzg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zndstvzx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xoepiyma.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jtiumuza.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ofaixasa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2tijvkiua.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlcdrnke.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hujtfkec.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2htxxpkbj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ipgslpdg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mlyzsyri.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2pbcytybj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqpldlek.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zmiaooij.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cdhvgirr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2loxkybru.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lneiiesj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewjeyaag.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yqzqulog.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lzndustg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2puqgjijv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2eiwcivuy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2shwvwcbd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kljxezhl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ckvrksrl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hevxoplq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ewurmctb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2eozbsjga.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2sltpxdgu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sgrgyjcw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kuqtbdih.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2whkimmmt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bxqoaobk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvhddjxh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnjahrwj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uvdcnkfs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cxipnplx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2strfkirl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lxepxjhl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rlbjfssl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ahhvrhgk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kcyypkbf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nlztkzxl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rzidhoet.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnxrtyne.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apwfbjrg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rwkheaul.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ykbwxjrd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uniyyfsj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cknriets.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xwaoiozw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nawtfive.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sajnzbzi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gwusjsyc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aexgwreq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2scurbxsk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jqygfoge.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vosyuvor.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yxoztccm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2obqtxklj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qkoiyffj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2olqfvbxk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gmclztnt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2velnmtoc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mophykqg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nsfsfdxm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2iwssuyvz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ujdkfqfr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lgywucqz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2donagkmd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lgajrpdo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgzlue.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ywvampvu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xvtirssk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2htpbkgkb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xrtqncfb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2skowhcor.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cygjmdoc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2twsoopxl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2usgisopo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ivjncrql.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2toudvtxq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2epwhtfpu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2brgdfazp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2quifacmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfiprthw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2womrkmcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybzrzhpg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yxjphkny.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fqjobsze.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zdmwrsxg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qytdnohn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsgxsams.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qvjlgoga.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rokqlepj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tspgcpuy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymxubodt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2oytzewyn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2bqpgtsyv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gcopybhx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtbnqcyf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyrtmfvv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kcnzdqpc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mffvbavo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2snsigwls.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lnvbqmto.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lfxmsirv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zlgsejmk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zucooixw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2orzusgcm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tqffahkz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2heojkznr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2phnzagda.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2oxoylvoq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zcdgpvzy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jpiuddhd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2egrejltn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nntkrbvn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hpswsxze.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kzvbwvjx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fduuuwgn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bjhgcbxr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yeuqtfka.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vldwqkai.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bzhzhtwy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2czwvqrqz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2uedjbvjh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uitlgkic.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tlykhasq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmbjremo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2aoibaswf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zspkslzl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2undwzyzb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jeoildsp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2saawbmed.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xowtaqym.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2iapuuqde.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nlqajdqq.html


<!-- 参考信息 -->