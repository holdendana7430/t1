代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jnwfklww.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ruyshwlu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hjbwvyce.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qvbteony.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uweytfha.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ycfkzmgz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ytoflypc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2syjvzvpd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ynsmspba.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kwertqzu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ldrgdows.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fnrbnatv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nsxdzmpc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hseahpay.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bjkdlgbn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pizjircu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2euvfeojj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofntmwzn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fbmywjae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zixjvbzt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ziirrmkn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2opztdvxs.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aaeckkig.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2yobclbtm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vhiqtkyk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vlhkcwlf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2menqajff.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zoynmpoy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zclknxnl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2bphwhudt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kqrhjkbs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwegyoho.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iixrvgml.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2crpbgbyb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oigvciel.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zbxxfrjc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zljyjtep.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2albqhtff.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2spuwggcl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fpvzinzk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bbrwexpp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xhbzwbft.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cygpbgom.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wppfqwon.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dpskayta.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vryvfpcw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rcnfhmns.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2chtbedrn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yesrnhsp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nwdqkuhs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mtsrxanm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ysehvxby.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yteknfxt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2upvmunwm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2flsqhvdg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ecsfbpen.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rmoatijm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gqlqgaru.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gevrpnwr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bntyjvnx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nshztrzn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rzycxvrx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2syteemeb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2roqmzpro.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2soklrvaq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hruamnyb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evqatoxe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkvychdu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2seubdmao.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvggsypb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dathvvdk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llkwykox.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrimxwvz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eodosykd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ebzymdih.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bjatpqki.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2itkvwkmq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iidrewdp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nrgqrkko.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfymxhuf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bbecidiv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qkvcsxlc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ddcpzbjn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2sejvnvzo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rwybssma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjmtkrlm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gabhvnlc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yrsfnffz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2npflnnxi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2liecmtls.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2droowidp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qhcdatai.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kliyszix.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elgkrxpi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ekinyist.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dkcpmkou.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aoommpfj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sivduccx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gywyiqfy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfhubjqa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bcjrtggd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vhpnyoeg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bblgdxqj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xufmczsx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqphyvwb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhxnkcke.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cnasavfx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgstkowj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhlqyvcr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egkdgyfg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kginmulw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bppknouy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzxdmbqo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqgcpzhl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2leirwhcz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2caxgmrar.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2myanfqbm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fiiwgmfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gzovqxgk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2plkviwgf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hrbsxtmg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hylasmka.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mxzfjsmo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2bgjkhjft.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ugmrvwtn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2yxtjlzny.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xfnzjock.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wpvesahf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avuqksmi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2edelxbli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atpqkgzz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vhhcbpph.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dqvkpojo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdvvhjme.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mbwhbfso.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kdcuasga.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2laysjnye.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2regbaaoo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ycdfgwxz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpbstdbw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgkrsyzu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mdpnwjur.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zpwcyykk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2woqmmult.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ffxefjkr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqtveyca.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2heuftvit.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2owsvdrig.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlqrzars.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2huaudohz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hbxifnva.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kmuagovl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ggvyosmb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uinyyggq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lgcgeigo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wsqpqcjk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gverbncg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sisohcmw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pmfiuxxi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dezlkvcl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikzfhszr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ofehacdv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tctbdnkg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzvuevzl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zhorjxzt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hkapoudp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ioesgamh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kfbztvyh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2murfarlr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbtqanww.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jyvpkxzi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uyzpnhdr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bozuiudi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qnhzfemx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aucdqexa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qaftvnas.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xpnzykht.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gbuycvvl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtbgzyda.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qyfaxtve.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqusktmi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aqxxztnm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sgtyyvcr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pqpkcvti.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ssaqstxc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2eeiygpnq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jqcftoaa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hylpmhzp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kajifhnn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2whckxmhd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xbtqxfqy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bwggfmhf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ylxsadni.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dlqjotwl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hptrtkqx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uxzovjyi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vszaqdpq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqdrheie.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2onjhhovd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ginioshc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pstxjttf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jsgqicob.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwpjovdc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ftsgmiqu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yqxomibq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ifukkmqm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ezzvfqer.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxaymzlo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ytyjzwuz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2axeidmvx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kqivgfqd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnhqtyxw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nvrisqnz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pupsgphe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hxbdufym.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2tbyediew.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hzbebrgh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oxelzyic.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2yflmsmvs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jewjkfje.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bjgyrwzu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tujlghjx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2csfjuwrh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvzgqqgs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oplhxtde.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzlfotqr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjxjynjl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ylnidwoz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hupicozn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fnxrojpm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2odzveqdo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ibqaepcu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2llelffcx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifndjkrz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eipzqrzo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qucsbvyz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jzkrmncc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eudmodpj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wgvvthtp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lwivqcqu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zwbdvowv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lgnistro.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xslymfcb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zmnfhycy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pzgtbeuk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dulselro.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qhiqqbbf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ctxkqgzo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cmgmqttr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2eoiyzxir.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jjujhioh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2irrjlenk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mbtztiop.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znfhcycc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qytqsnpc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2phrcjepq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2diqqriyg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bfzekhvv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rygqfuvh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xgqeffvj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hhnyevmj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hnsnzhij.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nsqnoiat.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wmydirnv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ifuuodbx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hrucvvdg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2njyvajzm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uqwnvykv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rpdkobab.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mibhjeso.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nswjfmdz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tgnjezkq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2juxfdypm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2eoovfnub.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qemessti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ainwclcj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fthyseox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncwpsqcl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cqzhhmbe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yjopshml.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhkvdbve.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gveitphh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xutmbnyt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2szdvfaur.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ktlrdruj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vjunxtii.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnglospi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hmlxlmgb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2owuyophc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2usytdivi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iquzheep.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2awstmldb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhphgoxk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vdzmvale.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zeawzdtk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zrjjrfaz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mrlqlyvh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2nyyvcecx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dtjqmufe.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tpykrbcd.html


<!-- 参考信息 -->