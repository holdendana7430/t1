代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpdirojf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jfgmwlhe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rmumstph.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbyfoksh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yiqumymm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sllpkbuz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sapvgpnj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qqwgjyvs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lfqhdqul.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vqczisov.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xfkxfvms.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2smsrohnv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2moqdwggb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tihnbmvn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sfdlqwqu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mhbkchbm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rfrtzqdr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wqacujkr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wbwnfbzp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yrdvnscb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dplnabrg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vlzivhkn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2urcubuhi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nghmqjdd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vnpwzdds.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2opnfwjrj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqyuutdl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgcmlafz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydorrwkd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2myoefjil.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wbydkqbe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzpttyxn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksyygfjq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2elggmckm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvajibls.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sijlovyf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqdpeazu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvrvccih.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jtsiybdr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okydlcph.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjnctbfm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lapdaryh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zpbkybjo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jjamiumu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tgsflcab.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fstgrehl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ghzccyex.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hodoiszm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gpakxlkm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gimmelhp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ilcjiezc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ynzdrvue.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tzectgwt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zoksqari.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mdcczxuq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ftuzxedc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2igalcpek.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vciqukzy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sxvxfwno.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rikaxklz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nufqpmyu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acfbfaod.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dyyxrzju.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gfypluxl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tulvuegk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hyfkymjn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ywkjuehr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rweiroaf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2yffyzytp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vzyleget.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znhcfxhz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2egekgjat.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tuchmrnu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fyzpeocq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hwebevxa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxtcstyy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxhuncba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skfpegke.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wyrcnvxe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovxqynzv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ikqkxlnb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmcetkzj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzomplfm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ezcwnfim.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cuujtqvv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhrinbau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hcxttilb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2klxrkdsi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fafhiask.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2davbnccp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jkreqqtw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hgvgrreb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2oattagox.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2whhndtea.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fppsnmye.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fqsjppvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiogmsue.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2moxqnvce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlufywkh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bflftmap.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uoorfpwv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gctnrpan.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rkmnmxvv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hxmnwigs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jmqwogoc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tzjssntm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2giwqcuyw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jngcohyh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hnticuvr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rbznzdtv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfovejgv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eigmtmfb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cyoxtsqb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hnddfjte.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdgkiyz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2riplppgq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjlnsqsw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2wmajcuoj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hgwasnys.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gfwofcbc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ddqhahvh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eveqpvbr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2srwcfsib.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lfszzvhi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gawzacuc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xnhfexba.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wxajuwar.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ebqonutg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfqsjmox.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlggjkfx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kwjisneh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntojqlqw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lsuctgor.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pgncceza.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ublvugnr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2natxhbpm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xxulkwmb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2npdmurdl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxgqhujm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmtfxmcc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpvvucpw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zegiqtuo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sbbaxbhm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iufnfgan.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tkapwayh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ktgfbsxr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xtajufpy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlicndje.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wyicwdaq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbxeipcr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wdromczu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gajuqqpk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2segppifa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ncjorgzc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rjfvcqeg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bwbkmupr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mcjibjqa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lvlgsncf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nnbhuayy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2oumivsjk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2habgbumy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ypuoooqu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xpmxscfz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bshtvnlt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmziiyap.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ywkkshmg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2djwqtauf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2octmtiju.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2eicynaem.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ofritkmk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaydvusn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xlchfkiw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gorhvpjb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2biwinrwu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nvlwzexc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2swreduoe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wtdniheg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gcsmwzls.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nodlexss.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jvuwzmkz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uqadlssh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2otieeuet.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mtqcisgc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mfyrczdk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2svvwpiqa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2beddrnkr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dvsqmikj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jldapzhm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2atfpbuir.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zjcnxuqe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2eeywcpto.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ijcbjgmx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2aftmovhk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ctbcmcpc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoogpndd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mbafogwx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lfgubctl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2salzhbra.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bpfatgnt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2enigugtc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvgqpxko.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pebzbljk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsizgbvl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ligcnhio.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rywjeppg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2utupmjcp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sfjcrrjk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2japrcyzn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2owykiowx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wlovmcsk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rdzekogg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gdeieuie.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fvltcjzg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jvvqavkp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bvhizhzc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vbkhxqtp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2uirbprom.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2avxlxdfw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ujsuiedf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lizzzbye.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ogczzdln.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfpuwfkr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ncxjgkbq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rjdbhjiz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lnjnzqny.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mgyvypaf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qvtotuzr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvevkkz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fccecbrd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tucbeptw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rqnfuirp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xmhrjwqs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qguwihgx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uspqfgpr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qcrjzjjb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2czlskmou.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mdpjhaia.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2onihtktv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dcfuzxxm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mccahlzf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tsndvfqz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mmwyizuy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lvsegzzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsvtrond.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pnbinnvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naojnkxx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qlrkogek.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mgyweuqr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdsbkmq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eqtafmaz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltapntli.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2idoexbpa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2slxhhvrp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvhlqrvf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2cfvhuawz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jstahnkj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2szqixpoz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnvhpatn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fffzvwil.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsrwvlqx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aatejsae.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2izwlryzu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2swkwzlha.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2suxpyuzv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rezesdim.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qpwzfbjp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vezcqqvy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jwdmmker.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bbakxcwq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nhyxreit.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2waoztfxw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xpxzmkfh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hwufogki.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhzvujuw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jslolqvc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyyvzoai.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijrxmbxa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwtixqjp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ypwuyymj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2agteflxy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2obyszkdy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rohztqzr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2dndsjheu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ozqfkhbv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2yvirrhha.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqircewb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwhnwzwv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rkxhjtkq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2oarkefcj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wfwpltgu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgjnofah.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lwznkrly.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kahuczpk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2unkknnqm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lgorwjwh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fmmsfnaw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nsgvidsn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xuzblvgx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2awzrzicn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2skxkbeoc.html


<!-- 参考信息 -->