代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gsyjcuant.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/ggujnktgu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/geqvczdjs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaepyoonl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gnmdzwgeo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gukfkrfei.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gxsnegogu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gdxikjsng.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gearocnnp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gmtaanzxj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gtqouupiu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gsmzilxnh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gdkyeovzz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gwyypyihm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gicbjmwzv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gjnxjsxou.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gchqzlgfz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gtqkprfmp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmiygvzzu.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/ghrpyzyid.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/geqvbkznb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gppksjheo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gocayeeob.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gmkqxemvf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gibowsjvf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gbqgjrhxf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gkrbosrnx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gjqanfjlj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gskmdqgry.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gcblieeek.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gicvhinqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbtzxrenp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfwjfrkvs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxeydxbkm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/ggtgbugyf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcsotfpit.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxmmozxpv.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/glczxqxdt.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gazspjnyg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwewlmpch.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/goaebflmt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpurrevsh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ghartlogb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gttrgrfsd.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmubioztl.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gsitynupq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gdujqfpmk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gqtromhhc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gzzqbauzn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gvdunrhgw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/govxxubih.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/ginyhffqa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gxujuprog.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gabrmwlwx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gabrxbxgi.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gsmelgvqo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gtazbpphs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gxcwfauaz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gjmvnfmlr.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gdskkzjbf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gzmhqzbhi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gehozijxh.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmvrvfbym.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gtizacdqp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/ggkveqndq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goujbkrvr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzfbmxner.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gocbauchs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gntpxwxpm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gmpjwypcl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gynvjozxu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzicjxoa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gyxzapvdp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gfxhyivao.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gktuijubh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gekwvnotz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gweexmgte.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcwfmilkh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gclgjvnai.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnlasbtpi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gautezahk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/geyjjetpn.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gmbserasp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghrkhmfkx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghigjibdz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmgfwhxcy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gegalkwgr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqqnwsvfg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gqkljirci.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvwgssdqk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gecogqsrm.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/ghrlirhyt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gajldlzew.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gsoibsbze.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gvgkjebha.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/giyvmioxs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/goxmdjmyf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/ghuqfsrqn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gtticazux.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gjawfdgic.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfvvvybcz.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/glukxuieg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghnkwjrhr.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gykwmuiyz.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gkgigzvjg.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gaypggeyw.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gjhwhnojv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/grpbucqpt.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gadpltzqk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/ghsanlnrg.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gdpzfudtr.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gwifrvowj.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gyzyvesep.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gbseacqkd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gqhlrqaku.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gnkgckjld.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/glxlqfaiu.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ggihordhd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gphpyxnly.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gfixoncbn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ggmbzxvne.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gcqxqdnui.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gfjeybhja.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxksbcsbq.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gjrrlplwk.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gwkqotjaw.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gvhlgbggu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gbxqxpbiy.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gbzthsctz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gmboaovnk.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gfemkjsuu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gwyzcgvhf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gospddkzj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/guljfirfy.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ggahwombw.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gfdooyuai.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gkhfeszam.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gcbrygind.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gaoknzlyk.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/ggbuvzabp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/groyuqqyi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqpdzudza.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gfnznynlc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gevfhxmdm.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gyvtskvsr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gnlyodyvd.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gpopljjeq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gcxpiludr.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gpmqsfoue.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gdxiskqts.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcyupzxzy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gbjjjrods.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnfeujmwq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gdkczcnmv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gzxiruvlh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gyabbnplb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gzkbrplgr.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gponogifd.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ggrhxidvj.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gmqpwvlde.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gghkxapzy.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbpxhazyb.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gsdjfbzxm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gvpzubtgc.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gdyiimszo.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gqkoqulta.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gywpkkipv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gmwqwiobi.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/giwqaitrj.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gebkcjeak.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gxsbvdqnl.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/grqdjpojx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/grngluunv.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gwvrppsvq.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/getpthpzo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gxdlthjgg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/govyhhvhs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gelupwacf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gonpgzhgu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/goeriuygh.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gkapbnpkl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gthnxrxlo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gtmyrgphk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gyxvthizg.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/giimudgqt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gyfowhvwt.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gekoyxcvp.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gnhyvruwj.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gzmqhbkqw.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gkipomgrz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gbqwdmwpb.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gglakahtw.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gjwqtomcr.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gektildig.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gxqimajst.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gnridxndy.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gizmcanjn.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gxrvgfexx.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/glzgymrbq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdgjctktz.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gzkhyqccb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gdeyckbps.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gglgjtlht.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gpzpzqtui.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/grhjveyfh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gfhqfrmlq.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gsfscykbe.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gccgundxj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/ghliqetkd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gzzwtdmal.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/goigdlucx.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/ghrzfwonx.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvklvzrtt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gwdtinuye.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gbcawebec.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtdgnvvro.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/grqnvjvvb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gsocaqyih.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gdxhemntv.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gssyhysxp.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gjslssuyz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gxcpbtvmk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/ganqzbopp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/glqmrudky.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gzaxwsapu.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gkonnogzt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gddzpwyph.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gegnofuwj.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gfwyyibza.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/glfzbmcqw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gqtbeoakd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcenkzqsy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ghyakasdl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gfwdzklan.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gvcsuvbbx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gktajwbva.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gdofcdaoa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/guylqmvkn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gxbxxnamo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gxthkxmjh.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gysoupywq.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ggtcgmkzz.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gvvrsplbv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gwnhgatcn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gdybfogzc.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gbgpscgro.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gnvzvggsf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcbeodhor.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gjcgbaviy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gizzwdfhq.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gxbngrmsx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gpuwmfeld.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gxdunvqkz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gtzqwbjeo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gjxurjexm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gutqdaacn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gmdbwwjcx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gdnrqbdjj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gmjinhoak.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gihqlbfoy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gthmozjzj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/goutadgrw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ggwklluuj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gimceifyx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gbkgaseha.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gsziwvtlr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gmnapizaq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goqlrfhjg.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gaesgkell.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gaiihchkh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gbzsltoew.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gixihcbod.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gcgpmpqnu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gvnfiexfy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gqrmrggfb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gmkngxsfw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ggcdvyuuu.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/golpkndgx.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gsllxopcr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gufwvdzlk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gnxfgvwxn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gjujqvptr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gylvwhphq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gcjmchsdi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtwvwovdg.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gdjcgyrte.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gkhhihiya.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gmshxwoit.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gqgrklkpf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gvtjogjgs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gxgioxtjw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gneqnyuix.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gaxaahmir.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gopwvotwv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gblkeivek.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gdyzdyqlv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gsuxdhkdm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gvdwyscwy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gifutoayk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gcchnccim.sHtML


<!-- 参考信息 -->