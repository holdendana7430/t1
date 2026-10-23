代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3icldtdsl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qaxehjcw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3usddtswr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbfjtwcd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3igpfivuj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dsjomtnz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3btsjalus.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pnyrivtj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3usbbbvvq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tttbthce.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dkuqmhwz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xxnynvqn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jhetlbga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dctxmngv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lzdftjev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrmzhvsc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pkumdksz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dccqhgkn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tksjiuyo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3fdcwpeie.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3glrubpzw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pxdjcjtz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xupwdgps.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fctiqyvr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kfcrrnse.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vtnhjlql.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uzhpoamn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhreibtz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bflmwvlc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xltkgjtq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qqxsluxi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3apncdgay.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nbwnjntv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3iczqtefr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ccaqvaqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lzlfysyq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vacmcphz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fmbjsuhy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kppadeom.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fqoksxfd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3aekzwgkv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aggdatsk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vozfejkv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3flackgvp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rrorqycy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rglnkwzo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3myxzvmgo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jxtzgvnt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3miybxpzs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mcpvwqzj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3plsllqgn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bkbedajj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3orkgbzns.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ewnsktjb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmrpluqg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fyincoef.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jswmsljs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3idggywxa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jbnpnsdg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cynajibx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzfkpzvt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pkhlkrva.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxmocjda.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mlasxwdw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyrmissx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdeejgfx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wtrfwwkv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kswdawcn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbjmddwf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rthjagtw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3apqmrffz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hndjuiyr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wtcplkfi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3acxezisj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iayyfdsn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cokskcck.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkboanv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ulaxucsu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rbtjlonq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tryivyuw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdfzlky.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kjoubfpc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tnszwkbm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jbupbymi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3godnbfng.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mrjjlgom.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3flushhbk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hechydyp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tmjajmdb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugaselkj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ardmldoc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qnhvvwde.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nkyhpfkk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tqsdxtbn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ihvvknwd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmjmqep.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jrxlcuyy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mkahcyzu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guatjqbk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rbsgllif.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihwfpmzz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zsmyxluk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qjtbvhjd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akhtwmja.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adovjrid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmznfeyw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jksswdlx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehlghkea.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pwgpcgmf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cixlbzij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vluimygm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ofaowhgs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3piqlcwyq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pujmubqq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ytioazwh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3stvytmkd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ddacufxy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lfvjxpkt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ujkotsqa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ifbyqgbx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qdourcao.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yuactbyn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uuoymrzm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tubslyqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szecyoad.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3amtqothi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtyjyjzx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ddiayusw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tkodafjr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zxaintvd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3obenjbtb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jsbqrghe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsuehmrl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfayrgd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mlxeamcs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucnejkch.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iinfwzoc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vvmipzjy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hkmkwpgr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wgphpmpz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wgdiakqo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yuciyjjo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xirxmily.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ndlsumyw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddvvnkhp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3eioxlvnv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dcpdntlo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ypezhrqk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hypwhtaf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rvtijqvq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pwlscbkl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3impwgiap.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ovdpljfd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gbfocfeq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3iseymrrp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mklunpio.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdqaumlw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nkwnkmnq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oavrhmib.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3huugijlo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uxceclms.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jqvofbrd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yvmmqwuh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zofaetrf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ajnlbvcu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3odfbgvdy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcxtwzmg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgjwgqjm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xgomdlkw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zvrbrfzx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3afgcffec.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3daxxvbaf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bqoyjoic.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ldkqlkyn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvfmjkao.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgvncsaj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ydybwidz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nekcbkdq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3soeuqcmn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mkekvkab.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jiddtvkt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gcgwjaqv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kgwytgbz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xmcgcujp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fkbvlwpg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zzymqogw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ggxkgawa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fkolhvgg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ktygbvpz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aprcprap.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bvadtwma.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tsshnysf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lthknulg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jqizmnvb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydfjkoaa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3btditjzl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ahjalxnb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uypgeres.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylqhmxys.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3htjxrxzo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dldvuqpm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbyeoqa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gosmawel.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3odquhron.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mdwnhzxh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3klzecdjf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sidtlale.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsahjchz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hmwtsjds.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vjvdjfiw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ftyyppvz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nnvuuhmm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ymstkweh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3culnjfye.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3komxbkog.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rzhwtmef.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nefroxzh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cccankha.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rtssjnep.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqwfytpt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fmevybir.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3buqpyqkl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkmpvfr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3siqxrprc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rcqytbsn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dzwwfpog.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abhlgduu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vnsjxcwk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xfnosvjt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3creksflk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pokbvrvn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mzjfgknu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bdjckfgq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bzzcfcga.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cvpgizsq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rmrixeww.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uyistlsi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rvlbipui.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cupabgut.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3crentscf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3apdyznfl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jyonottj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3guhndweg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vxkzssqa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3tnvsmziy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3civszgsi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bdhquiqj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cdirwswh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3virrrgvv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqovccja.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pwzrtoir.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3unwxufor.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qbacyuib.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tcduumvk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3oegkysdo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnnyeegf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3iclgzknr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hmunxjzw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vnvvtxlb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hvpsgyyh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yzhyneqz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3grkmutsg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3suijgjig.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3haoezpym.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gdjcnpug.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bwozmogd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lxjxozjo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tksthdjt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dpxnpeqd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ebbdhrkr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pgunkxhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zhoeuuuf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vjoghqco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxicqsmv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zrzvmqzy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3afzxfruy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwfrejnj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yykrqppf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhzjrksv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3psmmnvgb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tllaynca.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3beuhvyip.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3phkuvqay.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gmbvgyfs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3krdnzydu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rrpzlqmd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgnwgtlg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uwrchfkw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oitxoupq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ppxrzsrm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3nvuethem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dsiqlizv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jvjouvjt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3iosdddow.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mbuplwiy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gakqqwnr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qafvlkzx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3auxtcycp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zxkjrbej.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3worlgabi.html


<!-- 参考信息 -->