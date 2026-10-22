代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2abeelict.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozmxdivd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qviczebe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uthgvdfj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ershywdj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xymgprts.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mzcgrvzb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hfruqcsp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ydgjosgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuuhtwuj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ddqwwjya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyqkhpfp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ptwtgsao.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kmtuqpsq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2swcqgcdn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2yycsouzt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hjedbntj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zflxtapq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vocpnpmw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umqjkouw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fivsjzsp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kpizpqql.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2szafpxst.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wiwiofeu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suxtysqp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbcbssrc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lktadcqh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tgpohvtt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2qyoplsri.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pzhcgcgc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nfzvowbl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ppdgfohz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vsdxotyu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dmqzjytl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2esnycizh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hnchhamk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fxowlvlj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bqpxqnbw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fayltovs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnhjazda.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vwskilnb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rkzkrcyf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2frsfjxya.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2huqdcpwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nagtawfh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nxjdisof.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ojnisajg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ddgybgfl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pdckuzbd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vslaurer.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ubyfmhld.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owdvkzvl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwgfbtsr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2peycspka.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2swkqvxfg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yiivrkuu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gejxdiev.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpoorwdq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipizeadm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aadqbeer.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tatqxabz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvqpvhnc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2olvsexpd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgosnvep.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnytqnzy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dssutbco.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zayjhvac.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nfywsoda.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2weafpdvj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jkrtaded.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pkmbwxic.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ticfurmb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ktyaubfy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hdypeqkl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wpfmellq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iyvivquu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2baudnqty.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsovbbkl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pkfbfyfa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xrhzskdm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2urbkfacn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dxsvnpnr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ibehekus.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2doskqtyx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2whnclmxf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddqxjrbh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xcsvyapf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qvetssvt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iccyumnw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jklzpdrf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2amieefls.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ylbjpvgu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mpagvqsq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ckkwhwys.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypagfgff.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rferhihx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utukqtbv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxbvgpdp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jwdqycqu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2osqipfeh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idutfvru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udwlvpmk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gdesudtt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uefokgjd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rokttsyv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hebypacy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgfijsls.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ngjjqmjo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xdstccne.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcqwidwz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2llemixnk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2opldtpby.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2acdkrkbg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tdernopx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ijlialcn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nagldari.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nrhdlaap.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2osgbktha.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2krhqoxkq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fzxgmuvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oidschie.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mxbmmalc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyckvmch.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xxbojdlh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2utaursco.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lysydedh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2scssxfpq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukymovsm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kciblyeb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qqjhotzw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2chyiausq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2djppihvj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmvvjxze.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zeqlnbty.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2piwdwhpz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2paquaghz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lankftfm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2veaieyii.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2glxtownq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jjklyilf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxradic.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zumfddop.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wircqthf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lgcvanac.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mlieeucy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tjbfllhi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2djfrynip.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2syswcsmb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kearkzmi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2weofvorl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2akveviyb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zufzzsoe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bhrggjzx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwdnqti.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tnmgiiqm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwhsrayk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dqcpijlq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjmmsgmm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xdqvtcea.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2neogojuk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wvmmgixe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eayeznxv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qwobwjpg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cnjicrmh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuzxmxhy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2anblqoqc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tjseyjej.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmecurop.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dvdqftnu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gqxjwauo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2acqivkai.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2goabyqsa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jykaamsc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbuqoohu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jmbaezzu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2sziaescc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rbbitwmw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2phuabjjn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2arysayhx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jhurgybu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vgcqyxps.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2irwrnxdu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mxgfnivt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2idbimdmv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cpvwonec.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yngvfyqy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jxrgurfi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oyjkrrwg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2owxzuopd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcykkdxp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fhswswfm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbsrfely.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ofpgfnyd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwgieqfj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ztxavwfp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ixkxugug.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pxvcwdeu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nagprweq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2sybdihxb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jghqphrg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjwvute.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2oouohpvj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2whmctftu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgojostg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bttglrzs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ysaxwfeb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ulaibkiq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ugjblbmq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2giydcwza.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pgzbumcl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ltvnvqco.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vpmynrlg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oikqsiwr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dtghozqu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yirsbliq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fqbqejux.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkttnmza.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2khkkeicq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mcttveau.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nmzslwra.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wagivjek.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucmmafjy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qsplcroc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2beabjckh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cugqiodd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrmrirkv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwxjvmjf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jixisglx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uxajdvtt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gozyxida.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mpmimavl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cbtryvtw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2forsrfya.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rsmoynrb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gphlljki.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iaragmew.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pyglwsxo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wmtnbyll.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hbjdeqtr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kjnhoqro.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2daxjvckr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jgbnupok.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jgkxbvue.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cykcftxq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bsxmjsur.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdixvadz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2sklbnxgb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lgmialuq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ydtimxdq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2npotoumc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rsjguwfq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bnvldgas.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lriljqsz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sffkwsfw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wovrauey.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2uplcnlfa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jtnpnlru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2znsdowwu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2fyphvbzg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ynprxeqa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rixswlcv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jlnakmtf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rxwvgehs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hcuobnxz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kunmzbrt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2srrmiloe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lymznpju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snrzbszp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2svjcyswl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ioouuehk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hktkwika.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yfhvheqy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mjolclcs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rprwpgpk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ontpltag.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2tkznguis.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2oxrusdgt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bocrbqfr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xawaybzy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lqtghtcd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2recnaojd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gppppxsg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qfcpuyaq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bomqsdsg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mohlixim.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2elgjsudc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qrlztrxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2noftmbuf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tmxtyjjm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2nrrpqlmg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zrzahbuw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jyqfabia.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kggqpnxq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hlaeidcp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ertehcsh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nkpswktt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2amiytdfp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sjoyipeg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qqdjoafz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pdommpmt.html


<!-- 参考信息 -->