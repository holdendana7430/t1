代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dyzikkta.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2keuoixrb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bjqlffyx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hkqcoxki.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ckgaxfbt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2tutdiara.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yheysxii.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cyrzdggu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2utvmnnau.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ahcnolpu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ieenbhsl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fzxsardp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mcpmmbxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2purvxmwv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fcdgedsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkrzfsox.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pxouskxa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ickfqjvl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ebngvplu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2coseafzm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aszctaeo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ntvtnnbq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wditteoz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rodubrjx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2enhmkslf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilexwuca.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hdmzdqwa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhrlzndo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aiiowcoj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xhovscae.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vipumioc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqpyqngi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2csjbzvty.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rdhwoboi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ftntufbt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qqymmnxi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hyiehlqg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rcahaxuc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ayzgausw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lfavrcbb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ftzhytqz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oygrhcvx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pxxgauto.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rvbsequo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2higtlvbd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xztrqhnu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zpyotvnc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pdgseyaq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lkkdjksg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rkojfcco.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rbbucgys.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xtlhhqlc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cfxrmegc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kpfzvgjo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zmgdoinx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwognvdn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izvhmfhn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcbjrubz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2quyexlkw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azzhppex.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmupckdz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2emutxowi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krtwvbgi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2asapznhd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmwxgrbh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vyyeizzv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tzpujpyq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbickaht.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2obqpjrfg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2njvafmlk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qypiazpt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bsgfftqz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2striqjro.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rlpqlrzt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tbboficr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qosyygth.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qjsdeeav.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vpszwmok.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rnzsfqpk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rjnwlcug.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jttvmhgz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uhzffkjc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2inuhgoha.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zwkhyxog.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2riongpgn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2souiaoqr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xfeaupug.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ufwludak.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pkrjbvbf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkzttihs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ojlapput.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kyigayuy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ztzizdzz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzxwysbz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2itwkitoi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qweltnjd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xijvwkid.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vyvwafal.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izomgopx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tlhksodk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnblgbkv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulqnaxqj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bpejiiyh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnvejlbg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtuspwbx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jshpcgll.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ledcwevr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thudqlxs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rnzpnqzf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbmvknpl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iagazrka.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hseezyjy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fojfzavk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kypyfxlr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2opmfeecz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tjxyorbh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpdkhvz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gjbennph.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2plxnrtpq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cubgpvia.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2phlnwaar.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ibminlou.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yfmzrybz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ycvzjpiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppdzfbmi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jsvoajmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbcvzigy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hrizneow.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jewakfpx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2uimfxvhd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lovvmsqr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuedunso.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fqizpqha.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dwwrufzq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2inrnszpb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xivcrgxs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nrraekib.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2gkwnybub.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2liivaety.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xiefvniu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kaybplbb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xxsppftm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cllowrli.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kaztsjkf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppmcobrn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2deurkndw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ggrtqtoj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ixkgoclx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2phjsewub.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dxqclihk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nplwbogc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xtjwcmpa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rlqvwxkm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yoxywzyq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwafzvmf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2igytvmuu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjsipzql.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apyxiwdt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrkttacu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcrxniyj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tpxzexcn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wanjorgk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ujmezajx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wwmupejc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cjbidxgj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ocfwicgl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aglhvgyd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2leotadac.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsnifhdl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ysxmaxjm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2oulqsvyt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxymvrol.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pzpitiux.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2twlstbng.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnnlibmh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2upavkvqt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nkrgbsfu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rltcdpip.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hvtqbwsw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jfempmjr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2buowrhtb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oydoypgg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cnbczked.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ctdkdvmo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ihjfeyxm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gerpuyrk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2acapsgqi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bsczexbr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cznnkgnt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zxawkyec.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gbmilgvz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ywozdhcw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fbvrduoq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzrebbls.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkllrnmg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryaoelci.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vteltbza.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2emndzheg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnnhnqmj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ezwokwiw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vtfnmcxy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dmyxyjsz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2juscrrnx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xngqlanh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtnkzwd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2quojpolt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qjycyrft.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nmurozgx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2oeogulwp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mdifacaa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qtacnlyb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wxsfdvor.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2szilypad.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2obqhaycv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tglggiix.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tlalpaxy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2atkzaoou.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2newihcru.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kcvqdrmf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2csypixfl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtuphmjo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbvhutrq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ddzctzrz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gthpwgjd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mkmlwfdo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2onnqjkvf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tzrtxwbe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jktfobjd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2siwhysky.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hwdppifd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vinmvyfn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyzvdayb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2msiwgdlh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zfhahdsm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cfjmkfrw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2thmoizuq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2blowadol.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2subvsamz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pizyonor.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2khikuail.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nyszpzpn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kdrjtmxh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wwmnxqpx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fedkptcj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fuokpuyg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xfisghja.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2plmlexpc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ziwhqdiy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gupqjkkp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcoumffg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kkbixfgt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2pypmgxtc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2lznarkom.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2anxwipwb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ronfklqb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiftwozi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gghdmbte.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2whflwaat.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2utxhzdgk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vpvaiigf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2otfxcanr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dalhlhzl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2edbhbgbf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vzwtmuum.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wchdvgtr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mjfvsshn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2obojszcm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2emipsabg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2smykyyec.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ukxxjkok.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wrhgpaod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvrawezb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rfnmctzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liujrofk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gmfqdbky.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bzfpxxmm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2acbedrho.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypzekxwb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tvmkhrlw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlvohlzs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2vdnvqblm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcsuzfbr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wxuewfkg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qlbadgnj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2okqxamep.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vpxncuke.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bzigvugi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjntgdkh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xrxjxcbf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vocxcacc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2elrmbqav.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rhakbmdz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2czkvyzvh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gcfouqwz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rcaakzev.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sfsirfzt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xwqqgsel.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nawapmzs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2talneqjc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zeqozbmu.html


<!-- 参考信息 -->