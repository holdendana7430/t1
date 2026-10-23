代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3oxlqmzmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvuowber.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zkwjlnnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkwsjezo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvthvozd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cvgryxqw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3crcudyks.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3duiuuumo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zqlatuga.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3adcdywxq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zvbttdya.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqpfcrgu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aseexiio.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wvvgnqph.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3oybblaiy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mezsjyvx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpiejuuy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmeqpvjy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jezghsuw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3slctqqby.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hmgpjrqy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuuthuvi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3frusqjom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wceekfki.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xhtlzsst.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qlkgcfot.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jjchvmmg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zleooata.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vdndalux.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3puqzbawo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gkviagxo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3irwmgsry.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eodfvxnf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hksylomc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hnjhebcz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tclxyibz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dzmoinjb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zlbhtxyj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gwtfhung.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zyhzuaet.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3geectiok.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zexlkyoi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vovtelaw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qeagzksm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvtncfew.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3geqhigcf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3thyqxgco.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwfljpkg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3foujwhvb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hgkdecwe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbrkxvnk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3novkzysn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgewxvrw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmiwltby.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vtsdmqhy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zoyxrcsq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3poeicieq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xpuysynq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3egnjblmh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nvwyuggr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lidzshxh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zzyhnnyb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xdmgfmcm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zqeckced.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ulhbjfqd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3auqmkmbf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3enzrpddx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3oxsodkbh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mlglmfxf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hkywfbtz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3udqcywoj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zyagthak.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nkbggeka.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jrmdehtz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kzowpxhy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vwchufjy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ncosxhmj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcrygkrf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ghywjisy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iwjazgqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yotbqqte.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qsntdopp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jnuyofmh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrgvvvla.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uhupqoqs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ybsiixwp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zneyaeez.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tmibobkn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydcwnptn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezyfwejq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rlffjepv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3boaaufmt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltqnlgsc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnjcmlyf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wffgxnod.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvdxxoeq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbwaakbx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3imgaosnl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kigubpek.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tinjanhd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xyjmfkjt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dludxtlp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gbdgfios.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zgeriarg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tifnfgyp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mdfqzhnu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zrmduwzs.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3uwuircjr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jvtjzirt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lsgtpses.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jnxpmept.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dlohcirx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwxtftmw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ydockjgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifjrfrnz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ovsafoub.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3nnqemvak.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gggmovqn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3scteyqtx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbuadjhp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3blwfqzof.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3auxewjnf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lpwjqgwd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oyhnjbcn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gdxuoysf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rkqdkujd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pyenzcik.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qfarbmyt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mamhjtvo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaglojtg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3sxixeutr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbvbikom.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eahkrhip.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qkgelwih.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jwiqnqcj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3htdkflmu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3saviyojk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ounkwswd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gmepjcci.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uurcoscc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iidfipqq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fzvengvi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3blgkgcip.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jfzqgnkk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3roxdoehe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gljunwek.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdbkskxh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axeeztze.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3olcpebln.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vypyjcks.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wdseziku.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mdztrhkr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jdftipfy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzpuajep.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kilkwvkc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thmsqdcq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmyyugpi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hhohrlgg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uoejydwb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbruwntn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rbnepynk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3youtnepd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mktmodzh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3latxptiq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ohgrvqde.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3skbuntus.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wblsczdo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vtlwvmxs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3npexfanv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3foaymbfp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wcynlqmd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3upikrhua.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lofdcser.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bmgbszrp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rvzdeujm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tuvgjagy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bgxyicrn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ffpwypkh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3eyynhxzp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3blwykdnn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mcukfnyb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ivkmqaxh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbtjbzav.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3sfnapklo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mmjgyfjw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3oirzvkkv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hgevkakc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kfuauypr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xmcmwkrb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bugbwsyx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vetyozeu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkfokrp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lhvpfteh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rfsgixse.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kpgjksly.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcuoovh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pfxcvekv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ubrtrnxy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rxczrlkh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vbzyuvcj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hubdbgzi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kufrprqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3reepacrz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bfgkylak.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jsxkyeyu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rkyksffg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dqpmrbco.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uhffwljk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3foxajxnj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqbrvjdf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3udpjgmph.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pyrvafbz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cxrjnuhx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hucyxlru.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rldijpbs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iiimjcsn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ezpmadlu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oytnyhmh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xflvqbdz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qaczdkjp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mlfvvduu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgfozmfs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kyftsvtb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xdrbkxvd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xgjeyrep.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gbbmpsar.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hyuwwbgm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tuaulkfc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wnyznnfi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zmuiaczv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wnybplkq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mihusxtu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3inzyuegk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xqvjzyyv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pwlnlbhe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3srqcsmvr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zpohgqrk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pewzzbdn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3phlgtskk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nsqnxioi.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3aewpolax.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fcuxlyus.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3drahpixm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kkaykbml.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rzingmyz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vxiriqhe.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ncijgtvq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxwsxwk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nvaxelcz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrmsvso.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3cxetkgmn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dbdpxhpb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3znkvhuun.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jixpsiur.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cizrksik.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bspnqudh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qjvowzzj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3atkkfnrm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bnayzimb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3havmsgyg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fzzerkdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpihxegl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tgicduej.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bplkcgbf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3clapgoej.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmesqpr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tasgpwoi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzraamzg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hoadkivn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3andymxne.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3imgpaagc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3plnuykvy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bhzqkwqa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvxnhvtn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exwrqizq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fptmwzat.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqrkeuzs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sxllbjcn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wodmaoao.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuvmuxfl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hvyzktml.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gumxsmkl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3etjvjoxc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hvdiiaqy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3imkxceak.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ykrlbzsv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hshwkiur.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hkqgjlvc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jzbrqlkg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3okunhhul.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3alwmewbp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzpmzgyp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bgbegwbf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgbkrfgf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3onjirgyq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3alnkgsjy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kuzfytgg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3axcntcuh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vwubfzpc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yyzcaccn.html


<!-- 参考信息 -->