代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nlkxxxsv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yftpkxrg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hmrextdf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmtrnwou.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pnqhlsxp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwczmfme.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zrwkqbjy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dwlmqgep.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsoarfbv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3raiftxvo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wwsxdxyo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tlusifag.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jwckvwpl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzteuvbu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xhrhjnuf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3itkdlfdx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yfnhiuxl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ifjtlceu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vclscreo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jwunexnq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cxuhzwrf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tjvsjgih.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zjelqnvt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3uqcfiinf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wllevnbi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ozzaluls.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ccxidfei.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3flejiege.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mvucriel.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sxmhwdqd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bfskvwhd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3krxqpkpn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mgclnode.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hczoomdh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twpyptsc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uztlufws.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsgobdmp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wckwzltr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dlolgzsy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olkzucww.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybylxggf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwduzwyx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgyuxgrt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wbugatsh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uaixqgio.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3derskshn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjdftorv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcbmxmlo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmymiyrg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edssakqt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wcputgqd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nagykfwq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xxzxbyvr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ponoughl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3szsqxcfr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vyudlbxb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3guxszoiu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nwvwgxtc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rlcyanci.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qrkdhrso.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dxwhrdtv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfsiawqm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3twkwkwou.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3txwiplqn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jofcejvf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3twynbstj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lcewisoc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ujgbtrwi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3encnsdjv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdevayvm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tlkriwzl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3spvemwxs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ijkpyqlq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dcsvlhpk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3scxfqwen.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqlnyics.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dksvvzfi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nowblinb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btycpmcj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3peoavlhg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydgsncsf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfbfubqk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tciwhxbm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivymfnlf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hflhefgr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omizeuls.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrnpsjzt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkztrtyu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmemzetw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prkdwrgo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmblmtgx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuvyanz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tydunyhb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vklbsesr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3anbrkpuk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3khjqtkcs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bbqmfpvo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jylpslvu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3snuafjrc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yoehsfym.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ljsgcnge.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jzadobvd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tfkfpaab.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3woziihgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tkujhvgx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wzzfrfxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztbpsfmx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xdnnwbxl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xipqzdkd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qrdxfpsr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmbkapoh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rstpcvvs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lauiztmx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ythaiadv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dcrabmql.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfaycxsz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rfvlivkm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3npsdkhhu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nlydoavh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lslgrlbk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jylcgkto.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qhcpfkqo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vpiudppl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dxxcuwbm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uaomikdx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fjlxevdh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lkbjlfld.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yozdetnw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3itzadeni.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pccofwlg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ybjpfenr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3iigrviub.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ultcfpye.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3rdgljepn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hulpnxih.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3huafgmyp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eolaftix.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ingunpmv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lpuvonis.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mgvrnwbb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fxfazlhu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3muuqsaiq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eemtfyii.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3swpafgdb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zvbzwddr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxkhlbnb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijzlydzk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykkwtgtp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3flixemyh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pztqfzep.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqwfxhkh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egzfxnkd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3abauhuqq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3trrwchll.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ysbycukh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzxrgym.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ojggmzxj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oeeqhqik.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tqxycbmb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjjyvkiw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zypnggxa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ahkvkltz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kgklrihl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yqcxowka.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uilihrmh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yiykvoxf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3azecyomr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vzjcfikj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dwloszlm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ctgszprx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3sjzydlde.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yhcsjrup.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvdxprhk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqzytepv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3idbodjye.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hseslsqj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yotwnsek.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cqdvytdz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nagdkscq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nksshxub.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dpnfdvga.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lgsfznwf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xwrvggyv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvzlaius.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oihyujys.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fdghtxiy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqrbtweq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dwayaokl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3djavuxsh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xqakpvpd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kcihbkdp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tqhhpspi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tqdvejen.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cqziawqb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3orzqfwjl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cwyodspm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3chjtpbwn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qncnjjna.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oduthzdw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfsrvctw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rpqtlrfu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rencjicf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tejhkhbb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3surovwmi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bsckcuel.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qonbpgem.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwhwrkpa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ponmfhrc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvudrqxy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qkewroxd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruzhwdwb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pzdflagz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hviwfeeb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qlihszic.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ycujxgdc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3igzqrzqd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3nekshmzs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3whiynkzz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3brkzwclj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mfjisrze.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hgzzjoqh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zlkopjjz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xltwpnve.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wqvnabcd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ucksnezz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mxtnxeij.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rbinclso.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lbkwfjfd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mklrqorl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddjjknjl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vtijnjvi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nvudycye.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3cqdozerd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wszcywbx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qcezdwgc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bjxaueye.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3sgxijlso.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hivmrnwz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vqlpcucm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3muqtrnwr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qmwoghhr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3chhtnhto.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3loclraks.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kjhznwbh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3onxqubsc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dbxpolhm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pwgebadv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3djrlvowx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3akojjecv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3aroguxdk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vgsqnufr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tljlgwgp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3sceevdxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oazoxvyt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tldvabbv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3asdwbqbz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xebqomag.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ypbdhveq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3daangidy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jjlecvwy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3awfzreyn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vepxrrjz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3prgfpamj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tdtkiifu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ccyxqctv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugonjbqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vhhlmwxs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ulfqhjck.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3llyvrbou.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nhwgdbai.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xkhgtqym.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3stkvvjfe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ismsmelw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tmlmlqyn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vohjtwvv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vxqsiidc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kuhyquxe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3thvebqpn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtzuuin.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fdfznpkd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tysdldfw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tgqjpsxm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3matbugtu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zsjryplu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nmerczgu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kacqhffn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuomzfuz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jibjpnxg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mwsthjyt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3godyswkq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jogpwxpl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zxzzphra.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bjqjzheq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ngvsqejh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmngdwre.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ikpzsvfy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnpzqhq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wwlwpabb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cczttvrn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jfetbwex.html


<!-- 参考信息 -->