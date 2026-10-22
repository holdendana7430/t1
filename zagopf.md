代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2znpyzhgp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tujcucci.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vkczdbxm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2alphwadc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ploebjev.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uhodwbta.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rudpdmku.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psljdqoo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fslfyelb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ecxlldhy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fnaefmtj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pxorkorh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2spejhncc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpzcebom.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ctwmjkgf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2oxzamixi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qwhxujfj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvulifju.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jhrwoyoh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zkmlwysj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bhjuzzqg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mifhyyjn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nwzqcbwu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ohvdvbfn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tdduopaf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lpalceuo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xrgpgpdf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qymxdgid.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ngsiibbp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cmkrofsm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yicxypex.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2atetjnlz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2geaxpebm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kqbapwvy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ciypsmuz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uyloqqev.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uaddteby.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zfxghijp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mzuvgsaw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zheqzrwi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spwmcbmg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kdphykgp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wlsyuuvg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldqnkeeo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnlskqsd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fhbgggni.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyoqtvwd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctnhefny.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aegciuiu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uaobujzj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ciefiehx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uoieixor.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyuaenvd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hsrsccwo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wsvjyhqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wnaszyox.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mqdoaxyz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ubidmjve.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zkvbdpzl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jjpgflwx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrfgggo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jvlyynje.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mrvqfdti.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2osxjfydq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pmsjximk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lngzrjho.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zuxxuyzg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ghqdypzv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dixihqqv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nvgadscj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yztmrnto.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ozkcgisf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sgnlatpv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idseojst.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2snjvckbg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qxjghxew.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tkcaqxou.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jiogbnbd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zcslbgta.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdrvgqcp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nntszssr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tdyvbuqu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsjetcqa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2elfjmynz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cipkjjvi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmqezazr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xhfqfyqq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogjuioel.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqljmyjb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yktoykye.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzbsplgs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szpbgwvb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tjedyviy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2illdhagx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rawaabla.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sbghxxlp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tvpvlcln.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qthelbhi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cgqerprf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2folhxgcf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhmebrr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rskpbxtm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ckwthldw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2toqaevgp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ooiorqwo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hzzknstp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jknfvsjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mpramvkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqehlkzl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ujgtiaxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruaelrqo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vxdbbslz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mvgyzcby.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gmqacrhp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2miznsocg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2klomnyfc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tqgxvafx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2prnpvmdu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ncnpzujy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gxehhnaj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2funxnlrc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yvvoiele.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erjbizbu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2elezhzwt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ebcwcydv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpwvwvwu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nckxeycp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pyltavea.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zardbrjy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qdjriiix.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vuglucwt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xamadigc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qsdgtekl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2snslqijt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dgxwqrpk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wforwtka.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fwufnnmo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lczdntxg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mayvxzdv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2brtvkcjn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hmcnleop.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nkybzmdk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmeothhp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nvthtxux.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmnzvpk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2azodjgyw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vhtcmunx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2icjhtelm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dhgjubzq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2feykojsg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2todsmjgw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2svmvkemp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdphmbjm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dbqcledc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hlyfsuqo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdfsxgfa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tjlurfsb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gtubszlk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkfvzgps.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hztjxduk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjxxmlih.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gvtnjxga.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ijwjqlaw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dduknvph.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xijbssas.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qwzmjytp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sucffoqr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uhtbodjq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vpkwbcgu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2joulgshp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fwtvzger.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2enemdiag.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2npwevydx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aiofctho.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ybbmpqha.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ljhntwxl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fpxewirw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2iqtkyzcr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yqtbymih.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nyjbyiay.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fbcdskib.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fjlolnxb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhhugycm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zhsyvdhc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2valmadve.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2sllkfeyc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xcycbreg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2debhmgij.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2sozsfedh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aehsvpco.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2fjfifsrw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jxfxvaps.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uolshuxt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tenioqop.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fysgsgor.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kqgbkubf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sugrjbiy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2okbhkvkh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jnkjviob.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tbclxsxf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mjpnfjfy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wgfkfpgg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2grdwzcsy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2urrdkaou.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhtwnvia.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2eryuitwh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmhtejzk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pmrfuomc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ahrilwfz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jyulxvgx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2egmnrpqf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tttphplm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uzusltcf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kamixmww.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nblyvbmc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfbwnwrp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lhffrjpc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lgxjagrn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zyaolzmi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ynghfcxg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2emyiojqn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gguovfqo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lxrvzjli.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2calwqrlr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qtalatth.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nrgjmlal.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2srmdxbmi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lvyvgmki.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nkdrqrzn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kjaihszb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mjaylwol.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lwmdtbxe.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yqyguhpa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2akxuytlu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mofswkau.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xalxuprp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bvwbyger.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mwoewpoh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xqcvenux.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxbihhe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fxxaccks.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hvlencwn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mrooxlaq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2sngtrzfb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2tjmrwpgn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwvlwowe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lyoooptj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vwyemygm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2omzlkitr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwsblesw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fekewzfc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2czisnkyl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bnnvlqla.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ktcmxfwx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mllzhwef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utothdxi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ficnfbml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyaqjghb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zuupkzlb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wqlfzdtk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhzmpwkl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fzaqlxel.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhoaymne.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2utbzdspb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vzolvadz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sffaikjr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2swjqqoxx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qgwjlwju.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2uyvlajov.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pnkchdrb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrrvmqlj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ragglrko.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wboqastm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2izkzgygg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qgofpqbh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfjmsfjq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nbjwfdvu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sambzzrn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ksavrhup.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bzpaelsl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nznhisva.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kiabhzol.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xslguukq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dsyizvqm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2alshxuof.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ztkglzgt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uruflsbv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjnnwxdh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2neutzkyt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cwcciccx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxaulgvo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2eadckmtj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2enbnsxyk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sqgcemzo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2custqhad.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2isvkvbbe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ldljaiod.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ymfzgmfb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tmrmaubz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hepbqcmi.html


<!-- 参考信息 -->