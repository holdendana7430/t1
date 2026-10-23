代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3umskufih.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xkjogmke.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ksicymub.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfinosul.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3quzbknul.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkjfevcr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vtizprdf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyluiwee.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ngzcajdf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uwvabxvp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3spvhbuhl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hxndxfvy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ukldetvm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3udejggns.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ctefrdje.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3duijjjpd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3umkxqgng.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hfbvjooj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3emgyulsn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ojyzqqby.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3swhfmzue.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ujsdxiyl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lktonrus.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zxlkkwtz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pnajuvnu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3muqlshsu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pxesvufu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gjuswcsr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vubnggvq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xjahlcgj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovtanobd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bcsxltdi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3selxtest.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hnxmhpig.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zzixablj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqbxxfqp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpeeaanj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3besjjrhs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kpaaqdgo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azgoxwhu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzyevbrb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ouamaisf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfkklumc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ipjujhqa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zszpqpfn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhhybgpb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ijspduik.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtojamfk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxemukcj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ycfzpccx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3zoryiocv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nfadcluo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kkwqxvkz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ojvcmzjb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wpjpxbax.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rsnzaqyt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xlxymzkj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bxvvoqva.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hwvsvuun.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ocvjjoeo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3avwuxngs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3snzdmuxn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hszugijr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yxybjpim.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3icsfyaqv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vvjzteet.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cqnggsgj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pazjstyt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yglxwoiz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyksrdxo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oqllbces.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3apcoynuh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mozkemrr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rcxgaupq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ejbtlhfw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytqihctl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dludtisl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rfakobai.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epluiwaq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ubqgcoze.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjckdnkb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvjowrxn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qltxfmqx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wthcxmpu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmrrhfqs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awjxrvpj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlkxezdk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhnglmtf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlaamrok.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdtaedlv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmrfmkri.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewpppoby.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mjjzfurx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpudyknq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ovxupnmh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3aayonbzg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3irlocwmk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3incjbxee.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xfrjijfe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lrqvpuiv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ielcmmef.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3trxyjxiz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wiacjvyv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3chzzlthx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ziulfquz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uysfauqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trphxgok.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qemmsyow.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3efmqyyen.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vliljptj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ultjpfou.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvtwwtmo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mihsdjii.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vnempgyo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mrcjdiwd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tfikymsx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iijruysl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3dzycmmhx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3acnbdhjk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nzmgjwuf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fnbijule.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xgvqxseo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lblxkxok.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3iavyctpl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ihdiynme.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xzrtgqgk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kcgkqvze.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ptfmwjdo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ethftcuv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wahzpbxe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nfevrkog.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3aifbijbx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uwnuyraj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vdsyleme.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vslqymlm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3apidhrwe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejefiuny.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hytxgxpz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jcouhygv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nhbdoxad.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yknogxir.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kpirezbt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sivapdro.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kwsdvvrv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3elmblhkj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ejfamghy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xpnagzsv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxnefjkh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysxrrnpi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lcdfjxwl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kprkjdoi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3atllvefu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pkpupzzl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3drlxtlvs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mcqoxdkr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aziqpwgy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pspwmkrz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gvcwpreu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hyqhsntf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3skksgqej.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3eyckqrce.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rdnjujjf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mzgsbuto.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kffdnelk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bwlqkaoe.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3txlxvlkx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dekqpadi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pybemaif.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cjuktlmy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3znsqpztm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pwlvgmom.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bayedjzd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vowmmwpy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3oomclisi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckmpoxia.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lueuwpnb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3diudtxvg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3srxjtpdr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouidlxom.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nhdcrhjj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ermawqzi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlvuftea.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gqqiduhk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ywoesurt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xlixutlv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3msdutemm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sggumaay.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pplgroqg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3eqrgyaiu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jeqdsspq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3epqcpdoz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3oorhsndg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hgdmnyiw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fbhspykv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kxomxema.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ofdwfdie.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yinljuge.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hobwsith.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lzpnrtwu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cmeqeqxb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xklrcugg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnbqvmdn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdespnon.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mvlbdqhm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qxuroxzk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mppxugvv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upuwhtpc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3szjrptph.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ckphttoh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agqfamjr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdjztdz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anqgjbhx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hnefzzee.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pwmxtgnn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jnsksmbn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xsbnarrn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkavwgx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3purumwrp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ujfgnhnx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vexquylq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qqlnuyrz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3pekonvcv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gldpekdz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ognjenik.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nkuxmhhr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3elhfehda.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3evwjxczg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fwhkzija.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vqlibiky.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtqhzcvx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mvhwmnvv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bexaaiyg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3erixbdml.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xtpxrvhq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dbcpsmly.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwlyssma.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vgolodfo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3souqbycs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ajezbaes.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3aadnitab.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lrwsbvau.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oyqbncvm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sbsayabq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3iaewwaeu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3enickpkg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ylexzuxk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3znqwqmlx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pvnkwlhf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vkvcevvb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pwfisyvw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mjxhrgot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vafjiexv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3whdubdep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzdgtiam.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rhajnqgs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qdrbzjff.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pomknufu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eeklzfda.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kusuuaam.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzzcayja.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lnyoyvgr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3tqvdvpzs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kbrosytv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3htndvvjr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ocetqpws.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oikihafd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3epzhcogo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brhaqljg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hpsyuiiv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ywaqujfu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hjnskfmh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyxgdbau.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fvanuptd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3stlgjlen.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hsergzde.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yqiebhen.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xnggyqht.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cgbgrbtz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ryalcyud.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mmvesxsz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3frhlaltz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3errdcupt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bnmvakpj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmhkdned.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ospdomgi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yurhopcf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkfjnqzn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ujdizine.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xednjalm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fechdbvm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fplngyeh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ywrhwwut.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jwlrjafz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3oizcvzbb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gospnixf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3svzcbtkq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3bzrwpmea.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vyfpebhq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgfrteiz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uqmcwsyz.html


<!-- 参考信息 -->