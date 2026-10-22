代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2retrdpnd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuerrlbf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2miaeehep.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2htduyhgc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2sjtocivj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2skjmpybs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lerewwzb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ygroudyr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kmllfoqt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cmxomngk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oqrkcdvb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jzkznfrv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jkjxwwug.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2htnonyeb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jajuptpz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2uvzxoafk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2heagkkuk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2spippulq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axdxcavj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bvtzgdpq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mthfdcjt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vjihzytq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mswkhdro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2btxgwujz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2pchmvhhq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wfslthdx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ftiynauo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exmbqyce.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbfivczn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwlyuyqd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jfrntbgu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwbvbzkx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eizuxwkx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2knxxznto.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xharyvns.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eeowfmgm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lipgtnzh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whnyerhg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2awqwqmhz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vefntdqx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqdbdpth.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rlpbcjfx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2idfbtsxf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ixvfmymc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2degkdywl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2thpcakne.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fkjyiitt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nutyiodr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2swflzlng.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mwusdjyj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2obqmesjc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zfbsfpxq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2piuaroqr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qytvgnlj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2igqnljoy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tgonnchd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2piqoysgu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qdlretau.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fzcsjzls.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ebvaziiw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jtiyjneb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhzfljjx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hasghsdk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2afztvjdm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2axdtxegt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sstevkxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xvuuweax.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djeieyoj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tsdywsri.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mdaouilt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqfhjugf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqelazgc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsihrgoi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbibayyh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hqtevugi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2moczjtur.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2havradis.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkpbfpal.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvrkkbqf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fugroaam.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wmucqdog.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifmbvwyu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jypzdvrd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2enxtbvzw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yhbdtlrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwmmdwvr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fhuvdkom.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2skibgmje.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qdfdydvd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rbqxexza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2yulkhhmf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cyrvmyvx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2buqlczmq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bdmovkjb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vntqyjia.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bprojbzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rerdxbbw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lygzimer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lskhxxem.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2btvfzhup.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wqhexwzy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cxrlcxcy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eksovvwv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2swmzcfez.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bewpufwy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2naskubnh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2anskrrpi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpomnkhb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ejwxvcfq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mdqemjkt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vvkiydvc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nuqejppc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lktinvjk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmhfcugw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lixdpcpd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ghdqwsxw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pfsjfpve.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2idcqtcma.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yqenbsxj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sxctshxu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ijorbpjq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2chldwaix.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2edlhkjch.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2klgaksgs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2czxbymva.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lyrpizsl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qyywludr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vfezqywj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yvepkuth.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgmveosz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cssdpqjk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mgdvqnpa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2inxalnnl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nmfdjptr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vxgrqkkq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2juhczmfu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sjmazahh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2itgcvrmr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfvxwmjf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mngcdjhq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulcjnewy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ikkgehqp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2minmmbmu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bknxtvgg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dxqmfsup.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sleojnxr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uriqyxtj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdwurrrn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvimpybf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqcrnccs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2bwkgvktr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpmkxmiu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2npfxnzfl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qnjcumcn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xnhsiwpi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ergdvrhu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cgsjclto.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jshzzctj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eafwdldl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cjyenysr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2spvnajcr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2biwetvuy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wclkploj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dyxkxday.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsbsffnx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dujelnht.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlzpykok.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjosttvn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2geqfsoai.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkyqjktr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2oelhgsew.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bgorglbl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mayxotul.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yifhldbc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kmkcvzzv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztiwpzne.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ivhkeygf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sfrzljih.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ayvcooqa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owzluovs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2woathzfw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2takksutj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2czfvubsp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2axwntnwe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mzwxmerb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jujpsgnf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kkevoirm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gymhffba.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2epwgrucx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uuqgshcj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2akzhswxj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cscuayfv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jospqpig.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arjgbvqh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nezgjclv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2scfxguli.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qvxzllpr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2amviwgln.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2esuqkzon.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ccvwzogr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sdbuorbo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlpflezs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugxxxhve.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uesslzwt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nmfsynke.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwbcpdei.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lkoyawih.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ulesglcp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2khdeinbx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2drnzwlcq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fgmbejkr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mzzzzmyj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ekibjeej.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2luiuiigb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lkhxzrkn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wdsopzlv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gqlzogkm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2aywcjyhc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kyafpvoz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2epdvrjhk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tcddjent.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emmsskkc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pfeuqfrw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2htnuypos.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pnawnmbx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2woxvpvth.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wfgkhwpu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nemtljjj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rhfgbqes.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zhzegryw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ekmnakss.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ddendeut.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2agrmccid.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bgmplrak.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cdmbghar.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kmbirckw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qaxzytsf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wfhrtokz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sypuxabk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2oclaette.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2obgjmqti.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mryaszmq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mpedxcuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgwpkhfw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qnjhdapm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybeofurk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xzmeuhzq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cdpifziu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzcgadqy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rzorawqg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2trtdirpg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmksyeaj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vmgcefnh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2iujatcdl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mtpcotaf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tnskrbjs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cfmgybul.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hfgqsmje.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvvagqr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2osfrqbfl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhzjeowj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2oicezdhc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jbcxccnz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2djkssamd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mveqndun.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2inizgiwu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dckbuwjz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lpwcyyim.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nesuqzcd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tzyfpzxq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ssotdrpf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zlosztnf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2owdekhiy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zflvhnpk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2pgluoeir.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tfxcjsjb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojlvggnh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bvzqbtlf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jepllvha.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2aefjxchi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gklfblaf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohiwiscn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gizqlfsf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wbncrepz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wrvimuhj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocjnxgwz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zkmobkky.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbtecceu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wafnfpny.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oehfsmjq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajyizxkb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jnbqgugk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2shkjawjt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nbdpbxwx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qhofuirn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ojgsfebj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2eutwocmd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qstsxxur.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2saijipqm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wqfnyswz.html


<!-- 参考信息 -->