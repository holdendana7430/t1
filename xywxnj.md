代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3urutouzh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwblmacw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qsapxmkt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfglfyao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3taelugaa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3deopeaiq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bnkzknct.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3seobeyij.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lhscxazm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bowjzksa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jlclditt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3drwmslhs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3avjekumc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zlfguhil.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cgwywvik.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xdzmeqrw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3tmhkykmk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lrcdswsv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ucprqkxz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3smndalmj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zngudlne.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jgybpctz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3czdklknp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bcqvbsok.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bkyzbzra.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ndasfheb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdtiloi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yejuhyae.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ukneepjl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qifutuab.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3suewqdad.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvwspocb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvszowcx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3koqjooay.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3njbwunfo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytoxjbyr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xijvlmtz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jhcrujqd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiixdils.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjgzxomj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uviwubxn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iypvobxo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iduszdtu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tndlbnsc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wihtplvp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kakggjpb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lnbzvonk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rztumfby.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tolbmiih.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3reivxgwm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lzagdkbe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ogchshoq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3omcteber.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yzsjsusq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xuyugbiw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rcujbxts.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3otvnsuii.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nnlyeomx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xvynxvfq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pycphrje.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xbnmjghi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qorcqrru.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jvpsawyf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3usjkuwyr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ftoxfoaa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfajvxsa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xzmwzrng.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dnepyphu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wchpwvtp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qbvmvdtj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3nvkxiexj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrxkxtwb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jjqyntgb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3plgllkag.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ismtatjk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pfocjlee.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyaknumn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhzkyjvu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zadvasmz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cycmtioy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3galfekfy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuztfado.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hbqlsrxg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuksyxjy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ilyvhwfm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjcqnpzb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3syeihdpu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kpouspgs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dcldqbpu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsxcgvhx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3quewxsyp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lldlbljs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bmwajowr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ututawfu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xfgwadui.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mpnnieqk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3yisgrcmz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3wutcynit.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gdqhqcmh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3egjlqnax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcmjajks.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ndjecsdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhtoiphs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fxzyjgfa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qmwjocev.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tubxmdwm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bradsveq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tnamjydv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wusotzyu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hcgfxmzf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3sqofppug.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ysalpxhq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3upqcvcup.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nuhjbofi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3toapdckv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wyesckrx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnvhlbcl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fzinjfcb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vfdbdwyn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3smisfozw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ctgnnavn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3essfigoj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mvsjooyu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bcnrbbbh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xurcmmpe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ktvddftg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jgvabuux.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3thqtcsqr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zyifpbhw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bwrmwcth.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hvqhxzcv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ldzysmpj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuokobwc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jvqijtsn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pyxntudi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3joucsklk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qjtbpzca.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dnjzzxju.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oqynctuh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rztwiosh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cextwckz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rykgorxa.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rezwgeex.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fegcbwhf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eestbvhk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3krggokdm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3egnvxmen.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3elyrzqjm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ejmnxzsj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3racecjic.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oofjnxyh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sqagygpw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntexwdqm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gmtdenbn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tmtshmku.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3epmtslrs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3vadoenba.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3nvbnagnl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kdbgmxqy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kbwqtrlk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egshnknn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3guqwyvne.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3blfwdbjx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ogbiohvb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vzzfirvb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfdkimfe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3oifwmzkn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vzmrghyh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tcwjgnfu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nzxummdr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gamrdodx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mbkbcvub.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3moqecigk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dvrzgdjy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnxcuxay.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3odwzokwb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3llhjcxjj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jktyoslp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bxzcyxjp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3apdbvpbw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfqizdws.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aigfmowj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ptkxainv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkmerhdk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wlkzyzeo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kvhmkxof.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ycyjvbvw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nbuqwkin.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gmrzljty.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dzlijzgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zoppwstg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ildeknce.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zoenevxg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iygbodxg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tsbjmdfb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3edczyijw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3whuidpnn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kmhbbpet.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkcsrnqs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3prpwfdfm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pwvkgdyp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvosdnaf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cxrzlbpl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lwpufhcd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emchqyph.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cilobmpg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lrzprmqn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3csceunht.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpnzjfe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wpsntsbm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gnkxhynp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nqoifiiw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hbvgmjlm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fmgyyimd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uqywtmks.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yfvpehst.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fuogpvub.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uyoszcyz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ychkuizk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3iugdhcop.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ijlddtyn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dlmnormn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ogcwzkay.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xvawcple.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fkgbwdhn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3srdduauo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqcfuig.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zseishdq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3awkgmfbr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zyfptlry.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3igyknxbh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bhnkmnrl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fexicchz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nbtqwueu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3htqiakmd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3bamaglzc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jecycape.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rcatlfts.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3noiisiev.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3iicsntyt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3znnompix.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vsozjhya.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ylfaeyxp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3eymltyvz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zldnwjiz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qdkdxffv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vigsgudw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iorpgvdr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3qjjxspsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzqdvgyr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hpnqqcne.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nzfauhta.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hnfajtdo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uoxdfkhr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tqzoemdp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xquhycsr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gcaarkzv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3yadzqtif.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3iinvfoem.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fmpgdtpf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dyphtdso.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uxinvayq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vovlllac.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhixkoag.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsedzkxz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tidsgcqr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhzstuvf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqitfiwn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yeracgcj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3etrjfqrg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yqhajofq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bnxmbasl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ugyswano.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uoefxcof.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bojcnsxp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ixgwcqss.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ystrgqld.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ovmzbblt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mgtsmklb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xtesmnhp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ddpnihgv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nygeemvx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwbasqgo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bxqzmjhw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fxvtfads.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3woaqjxoq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3drqqrikn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tbdyebts.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gkucpnze.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqnghztx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwttcddf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnpbxpnn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3afmwnmkd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vryqfxhn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3uuqqcrju.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3omqhrdzo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lezocemk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vowabqsd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dheescmk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cxcpopty.html


<!-- 参考信息 -->