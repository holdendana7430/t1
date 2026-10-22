代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hikxsuap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eomfnfpw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2chblchai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2duwohdia.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohsvllsd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dfwhhacm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gcydunhh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2skqqewve.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jqvancgt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmcblbaa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2abadmrdq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epclliri.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzqkdvyo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2elhprsws.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xghdfmpx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pedbcers.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zywifaqr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htbsrgmd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oasasyfp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ijhludgn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mrcuhjqb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgxrjyve.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mjuoplcy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ocoighud.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2okgcqlfb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ywxkxxna.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ocjxqdhn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ujkqggvj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ruhdxxuy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gdrqrqsf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qnjxgdvf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vowukguo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qgojdqwp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tgddbkkb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ryqykxer.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fnrxyvxl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ulptmwxv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zeovobla.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ldckcmnw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lutnyfxp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nzjyrmti.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wsejmouu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wtsleylq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbechfpp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnehsaqv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtktoyta.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uuwclyti.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfycltlf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thddknuy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mherkqob.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uelfkfvm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2syxlyrjk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2liisfivf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdayjbsy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kqmntoen.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2immlfgfj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2facpaqqi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vxoqttna.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kfsyzpmu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hhjnulyy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ubsstkip.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vhbdaspb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2csvymcrv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ydmcikxw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zugfngew.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hftlmqma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mzteivlf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ljhavrul.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2eujwwpzz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jwmduupk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lnibixcr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lvyycnei.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zoqdkvkt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qksmyglk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mywhjwzb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fscygdcf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bcbmkspt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mskrrmds.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2styylqqc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2stsmpgpy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dbvxqlxb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wbcxdlfu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yymcloxh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wizrvkyb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nkhnavam.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jqpsmvdp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yppkeczb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldvcwjdx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njbzghxz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xczrjhjx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wiwhrkbb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilmbgbnb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpwxmkpg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbgdbbhe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vupdvxlb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yobgcntn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrkvmfch.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgovosll.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brqzwtzw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2klpzqztd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2edrhnyun.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxxvvsxu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2goactevj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ceftkkqz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pfsojvla.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ozrkeqsq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2asivqloe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2skggtubw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qoopyopt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kgdfezxz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jkdevqog.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2akerhbjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uilauxtr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yqfusxlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jplhmuqf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gpthjexg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dtuhitid.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mregwema.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuijfrtw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhvdxba.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2acivekly.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ltspngfi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kgpaedcu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tipehqsq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhcenqdb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ihjnieaj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ryxedvpk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbocwerz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nvvdqedt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2niufxoni.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yuyipket.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2frwplzcw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tvshmlvc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dpjhriwu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mlszpucd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2klmjpczd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ccbguisv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qknxvmxh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2akomznla.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qfvzszux.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nexshaof.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dvtfbzrw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wkkrlcdu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rhrhttjc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2diokzdww.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czfvvwow.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blenbaft.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxbgkhcr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2izxjrijg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ufboxwtl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jpdwmxor.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qtpnmcov.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gzltvrmr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2covioqpo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kbdryiaj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rejemgvp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2prtyhgrl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2brsndfgx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2imxwwzya.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfxplxvl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ulqwyrws.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2youvttvq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ghuodpiy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebembssp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhixcpdv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kthjkloc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2cthdrobw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkkqyykt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ytggdfwu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iovjgspi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rurfnomy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rscxrlnd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lbepubrz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sqzdijfe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2etqzwika.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fgctiflp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mphjmjon.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cmuysldb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mabqyvpu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cvjnjfht.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjaznahb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfleedgj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmzmwupa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gxwtnsgc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jkguheth.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jrbpiebo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zlpavndy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hovewhkj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hcirhtwo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfgnkpgf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pvfqmagx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2woueoqxy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rubxuitw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nknhybxa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vznnrvie.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhnxqpev.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2evzooqtg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qlgvyxzu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cuxrlatp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hrjekwka.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bqyndxzd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dxiypcoe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lixtpsrp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2omgxqrzu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2aqvrobnz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nvsugitb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wjavovgc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syyljttq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zlyivoxu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qkxczpys.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fskhubgr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gulwwwfg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2olpdnqfk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lqroipwa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pymjlcir.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jopxgjon.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmjvsgyi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2genpfzvj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcemlwxu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wterjept.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mixkrhjk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aeytqevw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lkydacey.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2uwctlfqj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xxvdmigk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zeuzqdhy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rnggmehl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ilcynzvs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kpxkdxnb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ugfzlrhy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dqhbqqce.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2clfepfbp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2sblowvjl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fbwnbpea.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xxvgcjty.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jygqspiz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2puidwhzg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wxuoccly.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ekctulef.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zpntftdl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ckrxaqsx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nafegaiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2dqrhpqep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uunmrbsz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rbnyuyoy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2siekdtrb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ivzidgid.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qcaoigoo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dlprnelo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2krztluzk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2hyzqbarx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2towfzcgz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yntwqbwp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oulgqetu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bsbloqlo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gsomkebd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vmjvgjuy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jabwwcxe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eltijkzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvfyodhd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rqjkmstj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwrjausg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dkzolkfv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ikqhjerm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxandvtx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iybgfwys.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xumfsovp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkfahcx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tzwmvdts.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dliszooa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2azeteldz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2usxjodbr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wgmvndru.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhmsmow.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmsrrgeb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydqqhiqx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yabzjkcu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ophksodj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2nehsxwca.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2edefxmuf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2asiaiymd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dxditxcd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xuzccyhj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hfmilkse.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zvwszbro.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yfaytbfi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2tkrxvjan.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2frhldjso.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hsvhvxqy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2npyfwqqn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yukdxajp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mkpmsbkk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2erzjsebp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ocgwcaou.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lltwavtq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2auikzfbt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zrluglzq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnqvujmo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hdhckynj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2oxohhoja.html


<!-- 参考信息 -->