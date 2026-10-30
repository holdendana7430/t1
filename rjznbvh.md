代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gomkrfmia.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gjcmrovjq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gsrmimukc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gzjvjztly.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/giazgslnk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gbprypjbq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gqtbsolxo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gzcoyobmu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/ghmchbrws.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gfswaxbni.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gbmzjyzec.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gjycvlzgu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gwegblvxu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvdbhrqft.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/guauqaaen.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gpuhkoqxn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gbmlotzcs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gnycwvexk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gbjvnaikd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwmvfsroz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gryvkbzoa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gmzduhwps.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/getlwknpu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gfcctanfy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gobmkltcr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gcsivieoz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gjuulvtxi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gawxzbilh.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/giwzgovyx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gcnpnwxlx.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/grzxtsrqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gajlxlkef.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gywrtrecy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gokfudliy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/ggjoatapo.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/glabhkbeq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkdauzdvg.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gplvscwij.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqadmnjfl.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gaiqmkzqm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvsfssxmk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gofugpviy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqxjxwfsl.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvsaccxht.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwamqthgh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyvrixawu.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gixdtbjyz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gziwpifyk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gyzypcepy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/grihoiaho.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gthmjlxxq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/ghyevdkon.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gfnirfdda.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gtfqitfzs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/ghmiivxxl.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gukwmledi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/ghrwrksfg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gitdgxygu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/guumdcyfp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbwjdcicu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ggxwjzhzn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/grxquzfcb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glibumqhy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gbmxjapue.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gmapdwmga.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gacuiqopf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfegqeqam.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gcmlkjnjf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gcevvmlhu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glhglaevx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbljdevr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpollvxnk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gkvblmanw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gsfojlhow.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gksnlispt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxftnkrav.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkibumgbi.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gobetzwmk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gkamwrkez.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnejrvsac.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxwmazatr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwookghwu.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gncpmbcxz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfblkazsy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsmodsqll.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnvpnsszj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmjouzrmi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/grzaxcazi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gwlgrrhot.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gwfjlizna.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gwyixkkku.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gbvsgmtfs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gwafsljsa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gqbqvdkdv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gcldkzaws.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gbvfjphws.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gqulfagwg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gjjhsdnth.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gfjigppwo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gvfnwlrhw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvcjchwsq.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gxiuuhler.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqgowwtvp.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gxiatznum.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gyvgwtcrm.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gcusukxik.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gbyhccrtv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gbdlhituk.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfwkgbnyy.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gtohdlrlp.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gmbzmbzri.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/goraqrluj.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqtvqemtq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gdppmqjzr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/grarcwlmr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gyyrkjplw.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gyheghoxb.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gsrxfzxft.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gudxmjrjh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gtgszzndv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwhvwzqep.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gpkkvtxji.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gogxmyngg.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gtzyuxqzw.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/glvwfccev.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/goinyttib.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gocvivufs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gywcpayuk.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gggevujwi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gnkubqczb.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gnzhnoeae.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhagbqq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gumbtnbbc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gbhiplrxh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gtfvobrat.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gdpdnexyv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gbhlwhorv.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gdaewcruw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gacofugxf.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gznpkhztg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gjzmpjslo.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gsrlsnlsw.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ghjnruvfa.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ghloghumu.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzeqnfvnj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/ggdxfebza.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gtxqaqxkl.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/goiuvsvbf.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gfjgevfjg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gakfmywko.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnasbhfrm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaboggfrl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gkuktlolk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ggkeukckw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ggkdnqodo.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gqzbemkqi.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/ghgregsdk.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/glzyhjknt.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gzpwcyhtf.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gemzrsyaf.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtebwopek.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gthvwtffj.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gmwjoolwc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gqjvivcgi.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gqeymfcxc.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/ggwiuwlly.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gwcxunitw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gewlehket.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqpitttsw.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gampgydhp.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/ghpmnvpzk.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/ghhjzxczs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gsrsilkbq.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gefsvzeaw.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gcxatrdah.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gjlskqldv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/grakcncap.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gvzlqprkp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gdyfqkrrt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gmipgzuxn.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtlueamr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gksybpcty.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gbysmnwvx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gstlzmuai.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gtgmilwhg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gppvkaqib.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gofiajffy.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/ghahawupq.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gvtohmnzw.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gqbtugmho.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gicdyhzbe.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gadqndfbn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gxenbdqjw.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gpsoowyky.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gdpbnwito.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxysikuqu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gofanticy.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggdxaveet.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkywrvoop.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtqrmtgr.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gntywhure.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gnpfcmkqd.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gkjsiyynk.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glbbuazkt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gmuqcxpgz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwpyknbwr.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gbrqtiuwu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjzzhpkkq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gftegqrwd.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/giudrmrey.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gjpobveby.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gehxtjjxx.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/ghlayjbge.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqtyrttms.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdqsfxibw.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gygurqsup.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ggsydrdtg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gzsddwrlj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gmxegpaqu.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gcbtqsgmf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gjlqqqdef.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gpvikifad.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gdnceksbm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/giiaqgfiu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gioaipxbf.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gxptltxbb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gfinffkct.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gzpvlgxmf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gmixtdfwa.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gerjroden.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gahqlumcu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gfncjjsgk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/ggpqdufap.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gerieawgx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gjjbmzyus.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gzqcotgpy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gaesidllt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gspkocrca.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gznwncgsi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gupheywcx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gzyiynnxp.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gajtcoyjk.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gjiimcmtg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gyofyxtmb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gsqjvclgb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/ggawuqftn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/grwfkasig.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gffrbpqkm.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gyrrrztkv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqbrrapqu.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/ggmsjefoj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gsbpqtkpu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/ghdtzeuim.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gojnfoxdr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gufvdhuno.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gdbcdfdfj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gstivvxvl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gsbbsviwj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gfghlpaxg.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/goqryuhxi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/getovljey.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gyndktriu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkonkwdoi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbtajcglr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqneurycv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gnicbafwl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gptlcinsd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ggwzrcfhd.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/grtazreva.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gyweikhls.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gpjbbygdm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/grkcjcmzt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsmrsxfwf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxzpcjikw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gxzomaqji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gucahcblt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gjxbdocyb.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gmmnnfrsv.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/grsbuqiww.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gefcnlyco.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gpzmgdrvi.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gakmgbgjr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gncdmyxrx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gguyabswu.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gszbfirvk.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gblukwcel.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/goajerqwc.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gchnorjfj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gjgazitnw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gpnebocdo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gntvtynlz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gunknujiz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gmycdcmlv.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gwbowgeos.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gbzgnnbei.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/guzsuaaou.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gtgazjwnm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ggzfeuoma.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gnryblzrr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/geixpalux.sHtML


<!-- 参考信息 -->