代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gfylxgan.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqhbekep.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zpqrqhds.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdrvahdr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pjhilpfv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xnytxoqm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ykeoftkd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vyhjhpsm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xsjotosn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jbkpgqpg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wmwncvvh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hrzuljkm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kkrywcbo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ysxgheri.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hvloskxf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3febhiulq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3frruapez.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wejcculf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rgatthfe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ahepjibn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qoqczfao.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hblnsmwa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yutfczkq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3izuuflqt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jjtngqdj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3klimwvgu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cgliwzem.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zaxkzmsf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mkyvvmsi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rbjhnmjb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xbenoinx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xkhrqqbg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lxwovbjj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xpnzaouf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whuarqpa.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffipwxaf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezyixsrn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3waoawtqv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qesdemmk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omaluupx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqvhfdco.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlxxpskf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3katrlyxb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3anwhhxnd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kooxfayy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmtqlqgm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gczofyht.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehyyrsre.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3goolclza.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fetjbmxs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3odplerkx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3npgmwona.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oocpczas.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lvfuzrxq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eandmnqr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nrnyjsou.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ppuamriv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vqaoobrr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kuppranq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wfitxzim.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jvyhwtwq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxhsyxio.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mpskjhlo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fdmdwjtc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sruzvqhs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tvgfrapy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ozufqhdz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gywhsmfi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3feethwsg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oafmxbvs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tosusaxp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xkuxcubj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uvrpakon.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3siqjxeft.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xvlgucmz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvboqcpn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ivilpthv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yafozfhy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvpcbmmp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iemcbiml.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjpfmmia.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qaghuytj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rfzppapc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqyejdri.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbosomtb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzrkrliv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkefhtwy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcosxtrx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3odobrvny.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnjfrzzu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dinnsrut.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3coziajyp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vsunwkcc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcniqune.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3peojxrbv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kxplbdhc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vooosbbu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jsqpshcj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uetszzkz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aookwzhb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3idrjdmtd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kqxwrftj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zhrbnvmz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kphsjeki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjjxnxen.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3okldhexd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idaijbzh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xheuynxh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jeoeovui.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzmqjwwo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrcphkme.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zmexrahe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjgacgag.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yzmbdtwq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zlrlkofc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3atbfevbm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uafiumed.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3iuoltbnk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeuquyqn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yxsefbus.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3umybuqhe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rogptieh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ldgcdrir.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nicijcoo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pudwrmmw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3plvlmzer.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rzhsssto.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ztfmfqkc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zatdahnu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yflvvzcl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pgfztifr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lessdsiz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kjyvkjzb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3oupmfvfe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3smliutnj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3almgqzsw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eviernyq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iklxxlpq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hlryoiue.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iznmhqua.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjglxku.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3byvhdsro.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3anwcchdj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bgwtjufr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3utbnaglc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bjxvywtm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkbxjuzx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mofgccez.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsrcdapc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ggpxvhdm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmeezppb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpkrwcio.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fbdagmjo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3accgxufc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqvwgvg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3piyclwgu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zymwsswt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bhcwohkd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rwehnhyx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jeyvruar.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3niyujndw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ikfmdnxb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vgcyczqu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wforsqrl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rjfpdoeg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3udsxkgct.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cakmwzrn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3edbsnlvy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kpjvwcfw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mcfzpxky.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cbwaivcd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3liifvzsy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uwznrsxj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkjpzmcd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ureynedn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tdzlqrzn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cxvxevpi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3igkcvnkk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mppmppqi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cwsxnunz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vquylkhu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ipefedkn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lhjxspxs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jthlddfc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lvcjeebk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lthaakvy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xvwtxgqh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsswkxpz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tuiqxytf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xegejkbg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fromfdsw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3whhaxxrq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vjvsuzkc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ipmkfdyh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3axhqagpr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oybgrhzi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yvkgmkio.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cmmryyrv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3htskokur.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mdrqocbz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nyjudufl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cupzvwya.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hhkxpzbu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lkycdfki.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3igrfcbnl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3llwcsifz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zptqutfg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bufsvykh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aouvyfhx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bteazovu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pcvihlhd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgekfppn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ldlenkea.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pyohmnje.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iixzpvwq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ydoxcbai.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xozuxjfw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cfesmuic.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vibhobif.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ukbuimcw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zuuhlgbi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3olygdygq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wuzbxnri.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3idbclyfw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3aqtdepkp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zrwqtrgn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nvgcrsms.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bumffyhq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3aayonguq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sxlvthlu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yuaskvxj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rphvtkmh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yuzcaglw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3awpfystg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmnxtkgr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3klrgekva.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wgluqlxs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmbtabps.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3goirlsxq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3cuksuhyw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wfllhrge.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xsevdyvl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3owouhuls.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lhfhoryc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gobalkfm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhndsvx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lmcnabbz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3osivdvxn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rufeimdz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vqumoagz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ykmdyxjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeiternr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gxewxrrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgiecibj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3newzrfix.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3atbmtnlj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnbkmixo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzrbtgoj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3smhartfw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yiiyixgy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bynfhota.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nntwzzuj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3megriyms.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fwmikduw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3iycawgnh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sytzredw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3judddjvv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pmitstgl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kzxmhlir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ttfqhxak.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dvvbjfck.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yktyxghh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lduskxey.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wyxgxwbj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3exaiculg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dravewxl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oxqkyiox.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mryibyrk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gagjldzf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pbayfkjc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uruyrjcc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gknozzke.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3woabzngx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgxxnckk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sigactkp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tsurmvqe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbiolyjb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3usrxhrhz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vwzzzexn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqrobecc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3grevqaos.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3oyyusiao.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vxwjcada.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bfjwqyas.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byrqzlbl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqgfyovu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dgnwwusi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3afwsbxzc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayglfwrd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kbbgiuzb.html


<!-- 参考信息 -->