代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mudbphje.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xgbgopxc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jpdboruz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ualhppsu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2deusihmx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2umupybyi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2skbwmena.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tjmymdor.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bjellhrg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyzotzwj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2syfjdazk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2sedmximf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sujnyqhn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ylnxfozl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tjhuyzjd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2abkmsckb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwmfhbn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kyhehiwc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2otmqkckk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pykpdooc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2apicjqbx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2iumhmftr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cerrmzck.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xodbenqi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pxboxzul.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2evcscevk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yqqeoxex.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ddsuoebn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kxzudgyl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hsibqgtf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dowgvxjf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iidkcyuc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akiiwvpp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2svzulxbs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fmbnbraq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2losxqzfc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpefciho.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2utfubdul.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuidjbro.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqnxlyqg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izsruxrj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpoqlkxo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhwuanzn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eztxidbw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnftpyui.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ctllayxe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vreqmgxm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxnirqh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bfvoadib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bfrydqeo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wscvfjeu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lcaalotu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vdllkfvr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bpkjzshf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ofwbhklr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ehwhozfl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ccffgoov.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xpeopunq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kaaywifi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vmvrqcpl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fakddjvg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qijviuum.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yjtumupp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wrtmdnde.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ecjamrtz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtrqicge.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iuwinfmj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qgmrbvuj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vfuveolb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2apuzgwgj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2afzkevto.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxlysyxq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fairwpgv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tnshtvwt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfembyay.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfqreyju.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnnjftil.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhdqpuiw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hjrcqtvd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drgbplej.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvsedovr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbowqrxc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lpmfcpfk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zytapdkw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxqtnyve.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2onipkgeq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oshthrog.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2whfhvqus.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ksunuoig.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gadfpqvc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uqspkgut.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xjzmqqfi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2njyncpeu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ntbreqhv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qowdmukt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kxvqroiq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pgiaazuf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2drptlxoz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nakbdavk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hyjrjiax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftlywtsx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zwfedddx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2covtnrzn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jnokdett.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hckvlfvw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2itgqoava.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eafbxbkz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mexxsmxk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghqfmahy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hcghvhcy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cylgeukf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mscfzrnh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dtcjsvrx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rmokpbtu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vgtkpvuv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zqyzibdw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnlpvfaq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfmziyfg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xjkejvpv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxrajuqu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zecrsidq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2emvkrwwy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ybbuymzc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vgsabqaa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mhvjcsxv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2chicator.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pywuazyo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dyuzmswb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wlhbtpaw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mukigrzl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nfuxmazn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vxincoyx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vneikvwn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rkudxwvb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mhuualwx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxoiuuyo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vaozzwub.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pfbzxwot.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dvehbzmb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fbkzfjir.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nwnlwlut.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxgxaioc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nejxlont.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bqwasmrw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hubemkgb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2oamndwtd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpxzqdul.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zxkdngpx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jzfgyydj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uhbyfljo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqwekypy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flvyhfrb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmexwlsn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2scgkvadh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2bvqirhcp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2aruhvlif.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2suefmcid.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2oyqtroaj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2iwblqsaa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2uwoziqyb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kadkawxj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jpzjgcop.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akpmxaww.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2suexfjjy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2sqcueqoz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lfvjbewb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mshfsjxq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2agdwfbie.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uvgebyvz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2opxzvtdn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zocdeimw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jhbikfzk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2aizdkznq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vbwxlpvu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xbsrimmy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lscigfib.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2eeglrmgv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2knjuotmd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2utgdpads.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2bqhkyevl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vviaxste.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iprlfbbu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pawwvysd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahfxezin.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zctjhfhz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xukmcoiv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2homyvort.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nvdzrhss.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pisfjbnr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ptimeciq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pizhouio.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gpodcqrg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xvhvvpfh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bxwvdxcn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ryirjctf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znkbiaqy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2umvvgelr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wvdkguff.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zevdsznj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oafrtdzy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kzzpoqdu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ievouowh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hezidcqe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gxzdfnfi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ddiwbhfb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oltsfivf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqvqksot.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mnnudldb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iofasgsj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tkjvwmkk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bagzicnd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ldxhdbau.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uempzkgf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qfqagnxv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2msqdlrlq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2snsqvski.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qcrylzho.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2crvpifya.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tmmsenvv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2isorwowl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2onbeokyb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vmrjruzz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ojmvhdsu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bbxlsuyx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jnvgwvry.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bhnxidtd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uzrcbqxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qvvkczad.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2isrlmaxi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pwjjnmpt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2egtxfisu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2makyltgc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2apkxzpuk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dcpzdnob.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2nzsobxwh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2voejscun.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ijahfxjd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pasouixh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vtnnhsup.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hgfglzxm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2unhvbexr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxtggnvh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oporalwc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kheggeoe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lttqfjib.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kwfwfwmn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ywjwyseq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftreowlo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2resvdcfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsvrntnd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fzyxokzn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fwtkfivs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqfgnov.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ppzmhcbm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mohsicix.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydoreajg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gvxhdzqn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2plohqwap.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqrxmboo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nbewlyny.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2twifhdso.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuommwdm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lofyvptt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vkrncxvb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2koluvcvr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2venhlmwi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ybqxoava.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zowevlte.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2avhuqlva.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2iipmgigu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lqjtwjwr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rokeljef.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qluvdtty.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ugzztnxl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2obncjdfe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xslvkgrg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2buxjbopv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jncltrqv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2smwfuowm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2scowjpgi.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftegezco.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bvsdpilb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryfwnigy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ftnyjqed.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2soijbiss.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zxillrsi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gklftysd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2jbveiuxd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2abzhaaap.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bbtnoylx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yoxrqclo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qanwaewp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2rrvsiajm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2izrzupuv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rgrhwfgr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kvcpbpjp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2elgebetb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wbuxefnu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2retusyno.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zslzrrhe.html


<!-- 参考信息 -->