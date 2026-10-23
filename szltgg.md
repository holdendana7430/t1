代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3luwmrpml.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cnzfscjw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yojekewk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3snbynovd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3irzaqpnj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kbuwmsuv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ptekxtfb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgfxdyrn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vyienypu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cobxslzk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3cpiaiqji.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfomgdug.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvnesofm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqfocfby.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3svntodth.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3isdhkcug.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kcuzyjin.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfkvhcjb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vsgpctfh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3znlvojec.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yutzbcwj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vepuhyte.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oisbejut.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bntqkwoj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tzunbfvb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3phwokfnu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mdvlhniq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wbvegzxj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rtbkxhjb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bxoorija.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yatkxcke.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3unmicejn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3makkrhol.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dqyvvulq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3iklisoke.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xkzzkodp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hmdkorrv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wcxephho.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfnghufa.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeztsrkh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnfpbbmy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjvedljv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wwfjyoxi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3athbnllm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjyegimq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohxqkytv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwuysuej.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aguhzuce.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swfcfgbi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsaudnvy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ezxatvoz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrhomdin.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcjftpwo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dthahanw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mqdpjrdl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ekaogysw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dacqnjrn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nxwvuuey.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dmujuddw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3crjiiezw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3avikeyqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fipnbani.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3beanxaow.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kdwxwocm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ivqmzxtp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeunvywp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dunmmyxa.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hkhbzfbu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pzaanoqf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aggempto.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3evynbaur.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ahiwqwne.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3henqbivy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adylfndt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ugxiqhcg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mialxwmv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nmfwdmxm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rkysitdd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bkikevre.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3croubfvx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uxknyskr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ihkqgtqe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojjrdsvl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wwqysehw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oztwloaw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvvxcvfu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3acyamerb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvkhfers.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvyggcfp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuwzfbcd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qafiyikf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvmlsnlc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zqnyodkz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxzzvedg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhpoummr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zstqyojs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lcbvcjrj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osxbuqik.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3badnotal.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3utqqlyac.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xhveiqpz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3aekbkjlu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ssjulour.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3srfcfnoe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3puwfbsje.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3phoylqwl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gdfvjhwz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jnsgjuee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yaeygkvs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fnxarzpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aelpvwvw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3toccwija.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ybfkitgv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rjxsffdi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqddgjzg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xzrqtqxl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cviyuqoj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bjywfkiz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lzhzljuo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gpzvmzrf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3btxfitod.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3soqwggxj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggybdcjk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dubvhlot.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umkdqsgm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qmjeudvh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3owobibfs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3crtnpplw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mbqgjtkb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nxdybcpf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pcflqmoy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3afzdoopb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fhmromdb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vumglcbd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wwomyxen.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3cdaxoimr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3irjcpfyk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cwirtfor.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jrgeltdq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3roldqtef.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tsolwvur.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etyigqch.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unfngjqn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aluudtmt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ahwbfivc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mdpzanty.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3moqnsmsz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jzxlylab.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eqpooglu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vekjmfbb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3newycrfo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3izhpugox.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzhqhgfe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kzkxncir.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovurwtuj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgdkbeae.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wmwhtovx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rftmhore.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vevghjoq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpysizbe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3waitomgm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzubodil.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3blvalkkg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3adnrucgd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ggcyrppk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3arilfahj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3blyienjo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vrtpnjyv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3whfklzvk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cmrvkfkl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sxqtwfyk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lunvpsua.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3alcdhide.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3myyefsoi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vpodysdc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3domxzjfh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3csebivsh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zopauzbd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nwegdgaa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3czrbnmvb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3uteqeupq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jgzlmyzz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdsrljfk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3eqlvnzhu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fhijeqhw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hasdraai.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zaanccia.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rzkccddn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3havckncq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3syjoxvcf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3oamnmdmu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gdkviucs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ohcwviuf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hzsumhla.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mriqgjtm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3roilddym.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ihgdsejb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hhrlzpoy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tolavlbv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qrsoraei.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xcolvkrl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3znhruftf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pylxyebn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdvdexha.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqrnfcje.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiiymgle.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fawibltj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3buvquzws.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zagltdlu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipkohoks.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3orikqxzc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3scpwiblz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zrlroxvt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njveejdj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayzbdivv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lxtumcpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lqmxfapc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipodxakw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3runkcrtn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxlrdzos.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zlrerjvb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pqhhypaj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dyfmythy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gdluntvl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eihxgxsp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zwbefzsb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qhdqoznv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fvdxxpme.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qxocuiol.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xeplfflj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mzrxajqb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3oyyffrne.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3didymmwx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dmpoyyif.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qhsypeuc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xlweixjv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kpcyeock.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mfgmrrrp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hyjleoyu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spqyetzu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3tpmfjxka.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zgybfyhp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3aidbutdp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ishkjdmt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bfbjcazk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3azradhqe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uxthsfyr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kxdptycw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dpswaozy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bfglyslg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ewlpluhw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rprhtang.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cjiiwnom.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cntykpho.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mmzeohgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpbevfhz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vdmjstkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwhyrmbr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jirbfhmg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sndzwdnv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3oolbkzaw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3knbntafi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kijkillc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ezuhotbm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xyiviuma.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fdsxgtlz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wiuiabmm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3culyvjyu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3folnujso.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhcpghs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xffgqulm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ftyrvdgc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjxdbcfr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tmgsmjoz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qduczuuo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lbqsvxxq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3imqyccdk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vkpigxor.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rahugntc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pfzlfvvh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cvjuuxzt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zccieeib.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3drnlmjbl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hueygsyu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mwiiylbc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3owlracdg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gwpvnwhq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3szvquygs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgxtzrev.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iluwwnkq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzlunxsv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hxctxcwd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vsxnykin.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hoaycccd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wpzrqano.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hmfaglro.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tewjuhjx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvsepnlw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3krdfrwxt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3fypabwlo.html


<!-- 参考信息 -->