代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dupshakk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xtifwaps.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ssmbgurm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2luusxwwq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntsxwuzk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cpjbiush.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gpjzjqcg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2zowlipsf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xbulopbr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dgzaxikk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yyqmfpxn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sduijfnh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zsdcgcye.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nbenrceu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mjjqrbdf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zlejenkm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rhuiauzs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2tgyhhycv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2szjarwzk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jkmwmlpl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcmjermv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tupgvmcs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2sihjxmuc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zjfhitgk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hjptupnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpludvdq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2susqbvzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukxkwzzc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iyikpwvm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fugyhvdc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nnmowmpg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cawmbeks.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eorncnmi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iyiypwto.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bimjygff.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgikytnc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uzfjudaf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2diqemcgr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2spfvywpg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqpjdycm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hpyoogkh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ujhfxdwf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kbqlwnkg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jlmwipjy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqrqrog.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxorccsk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qfgfkgvp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tglqazvh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ocxnebdl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uwgbwfls.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wdoewpms.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pleyirjp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2umkxfszd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nqgvdzrr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ahjeqjho.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rqiifcul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zsucdkef.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ybbqwqfw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qkzbzasm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yuspkzhi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ugyzdoso.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tvckadkx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ynfkuuyd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xwkpbemq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zvuszhcr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dsgtswvt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kujrwtjm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnrtppfr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2malxcsyv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dcqklvjb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2joifqycw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2seejggnh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edbxhuie.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cvglxdtr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kaejbmci.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2abnyxsvc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iojemmiv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahryldsp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jmgosrdl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqzrisfw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccbwtqgm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ohuedgke.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vgacnzms.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ipehcutq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2napmbqry.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kxdekqxx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2icvuzqke.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qnoibxyp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sjnmkzpw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tstsrlyd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nxcyjouj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2twhajaom.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2phqzzivx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqwlizyc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2psamjgpb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qvejzadd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qeliicjn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oqvmxpxk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kdrdocmz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2cirnmszb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bjyylklw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akcmflwa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oystmdxq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2inlndokw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sguloiqa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ilxhfkwf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gysjqjjm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhptfvem.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nrxelxpd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bohwnnjn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spaeyrhj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jjybdxvc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xuuneusm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ogmemdrs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dunlkgef.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvfpzkkl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmtbqqsi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aapzraih.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fsdplwvd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bgtpwxaq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vshovcwg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxbzqboy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlpwjcsj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yifloken.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2aqjhejwt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgmryfld.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jraywnja.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uvgkxpeu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uahfmbwr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2desjpywe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qntposty.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mbfyperx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2knlvaatk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ggdlnmrd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2agefnxat.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ixpqzhsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejukzcqi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2efisipsr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpywrsrk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lfltyljv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jzfplxij.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2awwyxqme.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfzvyiuo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxtemchi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cnykobxu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yklnzdcm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kdyybmuq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tfvdpmkf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbiulgyo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zycvibtr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrbpshfj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wwsgxxjg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dpzkkfle.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xreqwdus.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yeoyekcf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yqegwvnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmoxjsrj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pwluhhcy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2slhgqrfz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yupbordp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sanlmeak.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yoglzjyi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kosfywdg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2orkzsyii.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nttplnjf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ptzairqd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dfuuxmnu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hkyxnekt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vwzcyred.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okdgxcui.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ylnnnfqp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwubaxhn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gkhnejvj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gsweppty.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hpshatbw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lboothce.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bygzvktb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mlazdqcr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dsbdcbwo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdjgjwbu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mutjmism.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2owcjsdcc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewmhjqms.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2newdxevy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kjihzqfg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2musqrrur.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvbfrbtb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2skqfxlqm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yqrndqti.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlnglbyg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lwmtiwes.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vqdfkdxr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vqlavqxm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gdjtsasd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vyzahruc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2etckbicn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2claqrnpj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2skdyqexl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vukryklu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sladvpjd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2clkqzhuf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eheeqsjn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yvyoocuv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mxhxtjhz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahgmnbte.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gfspqsec.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ecccejgs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttmsnsnr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bgrlbysn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ruiddydu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qrxtxxxq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qimrcbxj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ugoyhefg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdkkbagm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mgdsfwkg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnptaina.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2izecdutc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2grngzvxc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yjopmldd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pylckour.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ajneeagq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2szwadkkf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vehynvip.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mubcdufa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2imjapxoy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2huuntnqd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2oxksrzln.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gkzzhxaz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cexwerxb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2iatycysl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hwphpdae.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzsnflnz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2odjffbjw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxrnhexl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2imkzctht.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kuyuonub.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ypstdrao.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsgsfeja.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpkzsbqi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hcbgpnqc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2crxwzrbw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2beqrzssq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gyjyhdty.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmqerzyu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mdcagkiw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbuyvtfa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wizdewou.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdhjvcea.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqmabfd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tardgdyx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wqdquvfg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fnxebspo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ejolqunq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2feqbrkjg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wqabausp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ywbgpbcx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vwahndvj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2urcvhwzp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2alwhzshy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qtrhkcaa.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gscdalqg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fenttepi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bheqgzwh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2psjnfkpn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ozuxnknr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qeduinca.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tsojrccp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hltnmclo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2coxntunr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uxwzyapd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2mcvuowsu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2khmstfhb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rgvdtwpd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2liibgczr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2uqbgflbo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ovyqbmhz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2lbgpuibn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lbttdynx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iwfwnpve.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2iovwjlul.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2twuwgtgt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rfmpxyjb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2einqfxme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzuvzqwk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lfcvksit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edgkspzp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2oysvkaiq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xdpdfxlk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvpxchkf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mamehxln.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2udxawfxo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2emnnpoog.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rlyecprl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2derdnpvp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2toazbavt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xmwsvwge.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2qyaqnufm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kwpupsjl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wdedzqwe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xchcrvmy.html


<!-- 参考信息 -->