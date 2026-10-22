代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltvwnljo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uafjlulp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wrafmbqt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2njlskeyy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2abejxfye.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2imidmdnw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ggutjozw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qgbhfgnw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aloykxnx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cjfshnlb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iaiaycvw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vdcznsys.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ptnayvff.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fjyhgacb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rjsjqvqe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xwemwnnx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cacxugrr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pgwrdylv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ygzjthzr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rfbpgjup.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tevwaaas.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lyqbzcaa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2avsujjrt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ecgvtfto.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xbzonahr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ielswdek.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxncliav.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2noifyfjg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqfwastc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wahzwtnw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qiymyibw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzjfjpbo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eelfzjcz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fyrjrukb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzawhbhi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzhpyhuw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyhkmabz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibipbayp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nyyfbqmv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpnunbok.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lclnthqx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kxwjukyi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zdzlbnte.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ojipkems.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tcdlspyd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hspytagh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2aabncfqy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ojeoaasm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zwkmneew.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ylmgicvh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tjftevrf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2iohabbzm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zhaqruza.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmiagrgs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eysvaonk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cqwlldij.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2umwhvvjk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fwtbmnym.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pvnwqeip.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lhdnzaki.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xunybkxk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqholcni.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dafneodp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nrwneoft.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ndpeituo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmqmotwa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2crwxjndk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tddyufme.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hderphno.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2arqfpnfk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2szviabee.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2duqrawgn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upuppjcm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovnbhzuq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2toazedax.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfmpyxcx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oysmifjk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjbwwhsb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhqxymqr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2voosfhxw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2femtuuoz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncdavhve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbklstvy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkouqrj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pkjtoent.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvbefcop.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2estfmvpz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ohmhdvnx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2eheskgbq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xbydnkds.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2eraiyjpk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vufotzwq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fivxuzwu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ninqafwc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ufnpgtmf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pdhqwocf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgoyyikw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fjdqwlfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkecjggp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2erqebied.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zniamjsl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpdbyekx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgwiigtw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bhsshpcq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ibnoylyb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2gczrsorh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kjpxpasg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atffxemd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgzokjla.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wsuawgvz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uleuafoe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wonrlnig.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jmxvwfsk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcpanrzs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zwstmksj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lplytswr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jxwatyzk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2owxstluo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pbdjireq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2loyjfyow.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ssnthniq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dgxarmva.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ofhxyilx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tlangdak.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cjcwdlog.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uefbvffr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2skiipcuf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uptjvibm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gvhjdjpu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhgunekd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wnbsyzan.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxwhteym.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kdpxosql.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2esoaxeij.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sjzvbrwe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dgejctgn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mxudxsfb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fgypllma.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wrejnvjk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zdmernoz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhtgpntl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pzdppkrr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2aixsgfzs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oacnnqea.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cwwwvnbg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2oyaiczyc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehonryjm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcqoxncs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqlfpwlx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yayxlbmn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kupnxgof.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdqegnve.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vakuxpvj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sqdocxmu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2plhqrjkc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2sbnijcue.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kpbjhcbv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iuugghjg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qvwgyuvm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pzrilrgi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jlcrxlae.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xvcihsoa.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qwkrerxp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rzouooik.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2cxxezrsl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gilywsew.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hvlznsik.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nutbxgkj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2gigmdxtj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2djtjkchg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tizyouai.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2uofghlsy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2krcjahgr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2sswmianb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2skpwtmhv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbkkkrib.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ojdnymxx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ryxklikl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oqfacbii.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqnvynev.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cwarcxhp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2efugldrq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2swqhtrwb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gmsfupcv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pkwlinjv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dxnohqvj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xmimkaix.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2krvotfnt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2scpsjvnx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qbsfyrio.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bfcdoaqp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sememfbf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2adelnkwa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nonvwyvi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zftslzyj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mkgzphah.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ayzjpziw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzkmcvrm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2andtwzfv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wgleqzhe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjsklqlm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlwtiaon.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uryaytid.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nniadazc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pfcdmgmf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajjrwtmq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zhfdjkli.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zemxpoog.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jxvfpman.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cbhtoyud.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jgamkznw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yjvfarrl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pawardkt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vqzzmbcl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rcrolkwt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yccorhww.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xemxtgei.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kzanwizr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ltjyqfev.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2igdjjmil.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2wnmlqsgm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfymlbxh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2upryrldg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2onfumvjm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xseglmtu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tvlrmzxa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2erlnaxnf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bqwuwqok.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ldtzituy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2utlimroz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2bsfpjeni.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nfrrxqme.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2kbzbrncm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yefkrnra.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jctmrhcg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ykjlxvob.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cjewdvkz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2filnuwfs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2melzgorr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qbijnnoa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cgxxgbqm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tadiuiop.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2msvnfqfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dndolqnu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mdgayfvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jydyaxad.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vdjghthn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nbolkzwm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpytlhwu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrqxudza.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2figptflq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylsaliwx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dhxnqtzr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ynagzpom.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2giyhgvlj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mirrpirw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zoyacpmp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iijeprss.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bznbnweg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bcyiivbk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2domdrmmr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ghicjjrm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hosvumyr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqjgrbfd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fetnndal.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2utrmtcan.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ukxwzyyt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rvxttybv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2veuxzgjp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oqbecojl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gnscjvly.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2nkdesiik.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tdlycqhb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftdbkfbj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2djssclyu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ybveyxae.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqurmwdp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jlkdgxdq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcjuzpqt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wyrwncej.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbjuydyb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2stfwsbrn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gjjgodte.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yldfhyrd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2iyyslyjx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtuzabwu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kraxcybh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilopmozs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2khftlsgq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lcstzcpy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dplakqmy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2hwwyvuul.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mlosepkt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2udcaylkz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wbqbdctp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kxjxorht.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kneadsuh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ahjlkhwx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2uhdmehyh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fmworxqd.html


<!-- 参考信息 -->