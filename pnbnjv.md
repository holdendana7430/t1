代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qzxudjot.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2pezxvsyf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2licscvrj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgczftyy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2oklvxeej.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tdgarjow.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iwatubks.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2caaksxmf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jjcrrwfy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kjjpyboc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mnayxvnt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zxnhrhzs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dmznudet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uonlljtu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fwqfttcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlgjszgu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyrjndcx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2aixghpiz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yuijcisi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nlxxudro.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yqktdybo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gspuizuf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2scnxacea.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irmfzgxt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nhlpwaze.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hliayedz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xecveheb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nitvnlkb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xwjbqpse.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezguzrkw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhgjpqm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dunjfsrj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qwcgzvyn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wtopiuhr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dbgvstjo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wdmfnmsu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vrfdbiaf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dovpsttd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ozeuudoy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fjxwcurj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jheaxqnz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2womekacc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2peyudpqq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2aacnuzmj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ofstmjpe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fpqphlpo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhywvhn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pdehqwuv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ciphqevg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvzkpkvb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fjhgaphv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lyztrnyi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2iyxkoumm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2boymsrss.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pnrqlcje.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rblmbefh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtiiebnl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pfplflej.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2oxdxjbah.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uembsubh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hsizxozv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mmmbpkde.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyahlmju.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wuaojsir.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvsseqzr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2csomhzda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cfoymzew.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnncjptb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcankkfe.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jauhnfie.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ntsytltk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wegipfqy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pfmcvasq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2goepipgd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mekwygkw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2thkncmds.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sjjvemut.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pzrllycb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2udgvnzug.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xgnruvni.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zdnsfxvh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pulvgkfm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cgxjcbpq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2czwlgemc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kegzrmqo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bqskqscm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gtzychkr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mubjqdcu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ausgggje.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghduhccu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cgwdsngn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lyrinrge.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cgaoqfdy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tjxhuqiv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hokzewzi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pippgdxs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yjlhdmwj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fvjmjdod.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yitzbesw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yhjjowhc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtnrycvx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdyhaiqe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fvlihwrd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdgjcufa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwjcjihl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqnwvlgq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rhzuqfgl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxfqpesu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xmltxbke.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrqffncv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxwmrxjh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bvmshwsp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2irnvpjtc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgrzkdgb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kyxgemeb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rurlxgdv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtwswni.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ctfxoysu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xvkocvic.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wuionzpa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ohspdvfv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hqfnhnqk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2twpzxpdn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fqfgtphl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvlcvode.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tydimyzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebwbnigr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2utkroier.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xwbtluxy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zwjanpiq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ndbhhxwd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xktffxin.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucxagehf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yzmkuokk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ikaaqwmu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bqzdaxxa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2niyoqjcx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zizwjstn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ucsbecqw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynvrmzog.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ldcllwoh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tgovukhk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jlihyzuk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xkqjrxhq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jwxbjzla.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tlmwnwbb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2axnxjofc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ocnvohvu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2alpirwon.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jflmksoc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2alfjrhtr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fzpzogsg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2azjivjne.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2twoyaulz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hvhzeljp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xbtgbwzx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dzkcgzrn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qcjwuoon.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jvpehhvm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2srkovolq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hkkarpot.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xfuglpyx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hnauphxh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kkvrhdfy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tqxcgdtr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfdgkvem.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lfdlymty.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtejnnrx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odcmgelg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hszealiv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rtywlehh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2batqgbad.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fpzllvez.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2plnlxcng.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aeryzmye.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xoeizute.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjtjpfud.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkymkxri.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vqrkkadn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dvivhnti.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2atpsvbwx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dnsikqlm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zqkbthej.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vkartnsn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qlcwxrdh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2htzjmtsh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sfjepxvc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ivrcsukg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cqtltxwn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tehvzqoi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2eqowbduw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2tbltfgnw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vfjnrltv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rhtrehmr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2askauopj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2apbsvgxf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dnqwnjzy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfnsagyk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2okanszra.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2akvasqjw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jutvrkro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyyokkgx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rlxzpkek.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2bmodtgmh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgrokxpp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lmmpfnqq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oifobkui.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amayoees.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gvjalivo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cwayptmq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mmvmphxf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ylctfwcs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zbcahsyf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2lvpwgjgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uaopaihs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lezfbfxl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dswqmopk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qxjkxgyi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zwvdsbbb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evrkigvh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gyjvizun.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kmrkuipz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2szfkkkkj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2prroxtcl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2moryazrj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rmgzvtbr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vshiuuae.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2brtwxlvj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oahstgkn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vwszzuti.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvnpsutq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pewtuwra.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pdnkjcfl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jblevodj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sczcexow.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2abhsybme.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hgqmtgsd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wqlgzfqh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2llxwdcku.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qhprltpo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bhfxhrbv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zkgvkwhk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qftkrpnf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2anvqisnb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mggbpbqh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kqbgbsyo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2attfqqpi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cfmxpguq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hdsjyqmz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2flutdroj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dnoxlbod.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2uttobmny.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2unieowza.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2evllszip.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ucuhqvzm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2npqjaunw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hgrbjynx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ncankeim.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2scohaygk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ktsekxvq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ubjoifnj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nyxvieka.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kpfoyyzt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uzmhydvs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2achhokqq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hmnngesc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2evnapzxy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yplzezyd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vckdwieb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2cjloxunr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ovpemxft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obtwnqwg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2aavjtesd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkdnjurv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xxywsgon.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lhtmtjax.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kizuxygp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcuhlgnz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjfgmwxc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhvggatg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2irsvonfo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijjyazkt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ijfxvwpx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gwuicymj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2klvdxhdl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbfzojet.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgztkuux.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ueuzuesz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zqzxqygd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2glrolvfl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fbwpybgv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ofwcldmg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bznmlpuy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2pkdbugdt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cciitqkh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fpxxzhps.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2elplveyo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2whcwoojw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dkshunha.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hdhszjyk.html


<!-- 参考信息 -->