代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tfbatach.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qudercsm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3fstqkdmv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvshgbrj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yvwqboxk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpnafwbl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3znhyvbaz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbzfkvs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecgbzpyd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svdiagbc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bbqbwdaw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nbhapcfl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ahqganhw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mepcdmvy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jvdzcwku.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ahgluyoo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xnsasloh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xfchsvmo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wswqefpw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3syicfybk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ddpcikqz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cjyalbtg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zdtlxkpv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tuxdswoy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3emszuoms.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fjphkggr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sgzubbep.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lwgkfrai.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bxhutlvz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zwqzauen.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ysfujfti.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fdauwarq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kitvdeak.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lcqyurro.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvwkevsp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxuulvxl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwrwxrnm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jlyusidi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lklaquup.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgorpdlm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upeiyuvn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbiaomra.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbcftndf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dgyztqfm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltwsaefk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3espjeubp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fjevvytr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vynyoilh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3odpigrfp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3epuouift.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3imsxcbur.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3byyjbogs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bqpecshj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tutmtyhe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rrkihzgy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3viegkdpg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qqmkhnfh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3sbbopjvw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cjzumswl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ruaisnvr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xqrcqlni.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vofnefis.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sqotjdvl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mmuggflm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xhevoyus.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ulnpzxsp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3plagelnd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ctiglpbu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eqpxsikg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjfyxytq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vprdigcg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bvyftwhx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3htlfkado.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sanrfazh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wuchnwml.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhvxhosl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gogwwmkj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rjssynfq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdtgecoy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tdkyxijo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpkilrej.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oobwssbf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3pgtdhbjr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmdwbyej.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quxtqbzu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxukimct.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzcieatt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsnaoegc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sioqyzhk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jamjcdkh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idanxkfl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wmgsayto.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rjjyfvft.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvibdapg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gayfmyuc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rbylwjmf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ejovovzy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pxhgkbwm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3haamhgkq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3uqwdenrh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3inwgsiir.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ucbiwlyv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ljoydzbx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rcskttpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3psbbwzoq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kwlmjlua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epiijvcq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3axxpwxlb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rprboila.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cisjyrok.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3goaajoln.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufqdzocz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhifjywn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sltxcces.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3aqfoggqd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lxmbtlqh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3byyxhexk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3didvauis.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmrkjrfw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3towknxiv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cstpplpy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceahasnj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3oikcdtkr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gaslmlfo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqmkrmxi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qnkslbol.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3goakhtik.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3optbdhsf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zcphloac.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qpmlmxlo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lssvnmzr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3izjhjlzp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ggpibwot.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3clywzczp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vrbhigkk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yoxbufjl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcrwcgwd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3inlbsqny.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uptgkzew.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zahvfxye.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sjadlzgz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3icimvdyy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ujphizck.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lhowchmo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nuiyzojx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3phsadivt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuiiuofb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjnkmbwv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pibwwqar.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hiwelsxp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3djvdtybt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncviazgh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pogrulja.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mtedwhfe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkmdzdgv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vhobdpht.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3slicvcyb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wgtzpbvj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3szsndpnd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3udsrjaen.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3deguvasi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tpqhxdah.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jpyvgcab.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vtwypqaf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dnbqgzrp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gqvszatn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3brlmgwaw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jvrnlilr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kpzbyeda.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wgxzbajd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qkykpwtw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3drrlyjqp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3triwrgms.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogzstwrs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tjrdpyaw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlqnivpq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vsxkbejr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wqqxndui.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zwaxjlvp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3gnvyujsv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mscyupvg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaielfhr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rvcmyywx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3smgdlnbz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3acurbiwy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfdevdcs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xhdvahvh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qwaumdaw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wcufxfxz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qsuzaqqd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sbumhxhu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vcblhbob.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zdmaiybt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jbjjelzd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3tzpbwsty.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tybchfoc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ozyrpwrs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ykbhshmh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jszarkqw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ogczhlbw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3goftpena.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxfjhyta.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afishxsv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dqusnhzi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jqavcrur.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jaxeyxdm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3apkgapii.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3crvstqvm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xfdkaslv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bicyoyak.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sgtagvuc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3imzpyhsk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lyooiukf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hbmobusk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gejdxnnf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qlthchwx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ystevvav.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wnnhsdei.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vytlevuk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3epvnmiof.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qwxuxqbz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vvfufggj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ioewxjfo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nxuwifbn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3yitzjsdm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xhvgoyko.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ttfsrvic.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wojcappd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rmzscgrv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxpufyds.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3whchebpr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wiviizhp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3towkuynn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qtknwwod.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ewauqczy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3evafyudt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yxmuoped.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aujyxsve.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3nbdgmbqe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nbhtyygs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ahgkenvd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3znxwhygw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3etssdbpa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fllylanw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wgndrsgn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwvriun.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jxouuxak.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3gcrdwkrx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xeauwjrd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3njgymllh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tptgetnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrtoajhv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zixmctyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpnbaclx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yhtkalib.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3chezqnrq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vzpladpa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wzfgflzy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpjydtpx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcscbxcn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nutnongz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rehyismx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mljnhuak.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3aoqwxfmt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3oqenkarf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bedditag.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkvjdlmj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qwnvubym.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhuzsvpy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fwldgxfn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dxqdczri.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxogeoty.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ckavifnf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hsntkmrg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3itrdtrxl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zfjiabzg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tjbzveki.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kztxsszl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dscqpgjn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kashycyf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kzevcmml.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3qtgioocw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qamahwzg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3opswkeys.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lulmmwui.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfozxnax.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uknsaikh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3aqyvdmhc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zwnagwnb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3bqedlerl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mzzkxxqc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3sakveoga.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3trkvadbk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xepcihio.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3twejtxtd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3klhhcafw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3gywiigch.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3knfiwxqf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3zqfcfpqz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ldjxwqsx.html


<!-- 参考信息 -->