代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rqbxfoqt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xadskwok.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vpuxywoi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dtoksjjw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cvfqysmt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2czyjbmra.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iuqanmuy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2krfcgndx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xvmvagzr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pgnabrhu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2izwyswkb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2njzagmjj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xuinofcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdefmwka.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ptcadyxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxetuonq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuqifejq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gdpidrau.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iehvjazj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2iohfcmsd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jpseurhg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2houyvzhu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2otagaaht.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehtdrmpx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2taxedpdm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bynkdndg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rsximoer.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2malergvz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbjgwixx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dldrfhzk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nftukxjx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lwtmfuuc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ckytiiij.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2igaaoyju.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gqwcbvko.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vwlwfgxi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2acveptus.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hyrwsczh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zoatpyre.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xkgxnazi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qhyizaho.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fecetjrq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ozklndct.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2oyeuejze.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jgkczcoy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2avzscpaa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aneagxev.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rzgcsfyn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ohrbczok.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ccghykfl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2lakpjcgp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bhuhpfvs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kpflbiji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qfbciqce.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2anbyfqqr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjrlbxbz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orgrlsyx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yzenbwpv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pclxotub.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nktjqmjz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdmdlipz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2irmtegib.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcehtnqs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2twtebyyu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2loixsytg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iltvccpv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2arpgebhz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxvowqfg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiozrsbi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mrdherfd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ddfsmesr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fuwvwfha.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jufwptwl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wzmdgzlj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rxshivwd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uvxecpyt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfqjhwu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2msmypfdi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ezwbbjuk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zsqnziws.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qkmuotiu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2phyqzesx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lelslwym.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bvcsqgeq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2khrnwsft.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cibcjmrc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jabomujd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ugwjaesq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kikghtva.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysgoaskh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iqzstoih.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kaobagke.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gvkgkofb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ortjbeji.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2stnspspa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncewrjvn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fbheelkk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vkrozlvx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffedzgmv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tmwymfye.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzfnudem.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usopcikr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ldmjwgfn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvavmlws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptpyfyoy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtrgrzex.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2drscayxv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iorjzfrk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rexkllxz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybqncdwo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydegktnz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aqdwutnz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2glmeaxgz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjjmcjet.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2veivjjlh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wjdkwgsn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ccbufyno.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dkfyjtbv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2abbvrazj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vwlgefhe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2abtxxvwr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2eqzvbxuz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uowcjfta.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vmrnmozo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppumistd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2agfcknwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjktflli.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nlswwnng.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2abpjaihy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tscgarmc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzxnjejo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ettwqacd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhylvzco.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fzdwenkn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2drzcouxo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iohzxqke.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2clhnlmot.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zeivextx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hduijnnz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctmadybz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpdpgaeo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bafvzsbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lhqhdoye.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mvyyjnaf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rsnosiog.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ovttuunx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nycbigci.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hnqxugml.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2isbrianq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2eznvjxid.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lrutsnkq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bfizijpk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iosimyty.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dwfnroys.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2igdumvzh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nnsdtlea.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2azqiufmf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2etzpohqf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qbyqrkgg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajbikett.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zvouflwi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvetaovq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kpatowyw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2plyjzrks.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2icqruvqf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgtghwtu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfqamwxc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bzbgcygf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmyjzomt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2eiuewvzw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yoesjkxm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcksffcf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tbsvhypa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tadgmmkf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gcfjmmiw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrmumvew.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtnszqul.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhnmnqis.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tbmuehpp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2erigkhii.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2agshvnpf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2akkytabn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2roabsoxk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bqalkqad.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qscicwlf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nnrbxsoj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fhpekdtn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hteifolm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ykmrunbn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vexzxnmy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iaqrybrz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ewobzjno.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hvfcfkve.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcpxseoz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvjybgic.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2thjduqtl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2eugfpovr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2neffywnb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhvgpuve.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bsulnnkh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2prsmmyph.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcvllubb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2aszfetrd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ztoiogzz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uipgqfat.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rqvblagy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xnmcxtbe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rctvtlgz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qeknyzem.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tcppedql.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mswnyywn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kupowjef.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uajznxkn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2njgsikbk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dpewhtgr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gcywuvua.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2znzyjgzl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uuoknlmx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2obvygcgf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfllgusf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axvbyadb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2meeckgyd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcrhuidx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xxthsdna.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pnhcveup.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkxdtyhl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tnrjikjq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bcdikkws.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppxfwlpk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2omomdddd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lqjbssso.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qnneejvl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jthgetps.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yzojniwh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kuuckwgh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2egwszxpk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qcwspeym.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ngpzxdzx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lulocfyr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tavhwwrq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2btxqusxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fkxcarwu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tltqnjep.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vjkkunmp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2plvffrwh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yxvzpmbc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ooifwrep.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wuxvsrtp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2iseigqiv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2nzkxxxao.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nnzmnqyh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fjqlhwtx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fuuximzm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2chazayyw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jlvaldkz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ozothrxc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vnewgrmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ucqmdldg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wezjrpla.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2uusbfara.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cptimdfv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ybqctsvx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rbkpjcja.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ybyxldlr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xfobthmz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mnoxvdml.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ozynfvij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yeztejam.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cvmaqouh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pzraaesp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2flfqyaqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmtcfppv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zsegmpub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfhhqqet.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2okydizei.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mmexkngu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iwpoelut.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lipkfvch.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eelzejnk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2adeeoahv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jnaswaxj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bsdghilo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tykokzpb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wbfuksyv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yemyngsj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2htpfpcjs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2skoovgup.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iuvuywcq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhywhme.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lqakwxhn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dbrhunri.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2widdgalj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rfyzqbyl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mooetesm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2avbdktno.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yzuqoxuf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lmalnkqz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qbhhaolz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ehwonrfg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ejcbjmha.html


<!-- 参考信息 -->