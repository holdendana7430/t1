代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrbolut.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wxbhhtxt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3swvozhpk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pjjfdvpj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3efgakhjp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zkteibba.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3stqobptb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jjflzdoj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mfqpollx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3sdktgefg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lpmkqwvy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gxcheods.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zcpxlyln.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wyzgtioy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aejjhtfo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3grfmnsav.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dtyjtagg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3khduuxjk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ceoufbbb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xplqhznx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dfdrpqor.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qcbruxcw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jhllfydv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ptaahvty.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fqixchhl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jjikpcfc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mpivsiie.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zwoilwbr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sebolwxj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3joijaush.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bkcxpmxj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dahserio.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vzezmknl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lebsimek.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wxwleyab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovbyoaja.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjgaswdc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hkviaeqa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbwsibhu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3eobuxxht.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jjsefisp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nlzodyyk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3avzughvf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eymqprle.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwhxkbhp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dieyosyg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bekxfwlw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3sohfsajh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixokrrlz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwesgckb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fuvpnxsb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yuecxcqi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uqqyyuln.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lkmcqzej.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3vaqrfomt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3iwjkpfmf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cdtybrcd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qvgmhgvl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rypwezrt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zxsdikzm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bccxoeny.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vmntdkcm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vdlagwse.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3pizphurz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dfcpblrz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3yioyrsbz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wsnlolln.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eqzlfdwn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3cphnlmax.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gwohecuc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bkgmzrgl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3csgqxmjd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nhbqxyvn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kpzpkwps.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kagwdjab.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyvyigpv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nsuklxoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bqkssrjn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gntzcytn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3heexdumk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlsuyazy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3aexqijif.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3godbyhom.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tltucjnt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjolgshe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnqwbxfg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwhhjwyp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pipszrde.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvgmbatx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxlnkoqa.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yvnsswpk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hziieuki.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kgbqwnfw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xiebrxlt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ucjysixj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ygyrnyzp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zinwyzsw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wbchszow.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3phijrzms.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3imfvigph.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hvdoasvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mckhempx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nxzbzqkc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zpdriflh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zlflaxmz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fspjjjfv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3msvlzsgy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tmgfwabo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kmeviokg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbyixjek.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yzdraala.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3blctkdxo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jndlyqmw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bckbmyia.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jgppirwg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbmyacsf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xvwpcrnc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3iefxysyj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yelsvcch.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dhkwjiuo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gginndeq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3beywnsll.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3zvaieqss.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3epptalfk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bryntkgr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkldbzcr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3yuyfpitk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgzqlfsu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zjcwrjmv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfrsahaj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbtzwlfx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3scnjutyy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3leldxbdz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cikxdcrb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pgxdxxth.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tycquclq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jllvhnpe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nsicxzfg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3utdrqlxo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pnlbltto.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ncehvwxt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oqmtkuab.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3itjcnojz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kpqvbzcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erdlqfzh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cqfzsrmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyzbuqlf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3llsfqjif.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3nbstbfbk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uulcuekz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckmvwkzo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ucuaopgs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vkqjewhd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kitotrii.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hiyhceow.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3crjeikiw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qrsyriuk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ajxsocub.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xykvigzb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxvpdves.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkhmxerm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gccxpqau.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dkdazdti.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3utbdgihe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpyihvfd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lmtmzspe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rgbscewo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zjicsxfr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lfpwbmwc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wholbvse.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3siznslbv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kijpqnyq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zczskyyl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3udlpuhtx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3iedtkpvd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eistxlxk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ahvygvcq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qajbmoep.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3aukujtug.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjgjtd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kzaospns.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3byzuargn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uxxqczrl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mnojghmr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3arpoillu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3toubeimv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fgsbtimf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qynsurae.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3efhkeusw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kbnezyam.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eiljlxjz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3lwaetkoj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ppzmoyti.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3sbqqjusd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ezxloxdk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pipfggbr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhtbpcvh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqhowtxg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bokjqesn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3trxxzgda.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3dtendcuw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cyogwfvp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bauunvrs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3krpzdvvt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mulskcoo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3htrlpsmv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3syfpldtz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3sjciulgd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mzqqtoku.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lfcdxuav.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lahhqelm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3sxutqjeo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dawnddfe.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaygzxxb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivjmacmo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ftlkhkpf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zgqyjwiu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mmzocgbf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dptpfmrx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3smmfzwdz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3czfwaiql.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpoywtek.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xfmhypsq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpamkaer.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3htyozjob.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xphxlamq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3avertdvx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iylneowt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mtdsxlul.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zylblsjg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zwukvujl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mhmvppum.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iagoyylw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pkvqehnc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3thokowkz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lvgloliw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ofburzbe.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3scxlcmwt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kbvksmrx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fzqzzhra.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rzuyezva.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ptslirtq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3osimlcxw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3egmfdisa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wbmfouue.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xktxjbiv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3monwciya.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3byekvosp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydczyulk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocpotsxu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sddypxwv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3haakespq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kkdqgytn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jeqziqpf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fhwbwmhh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kcdibqew.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kexromfb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wnpuwjak.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mnxnanmp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qjsnjbaz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zorxjfjj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwqryxds.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bjdepaih.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3soupsgta.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zeyvzhes.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qqvzpkoq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lafyceni.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pznqkftd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3oznbdlih.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nldyadnc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bqnyhvtc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vgpdkfpl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cxueyrot.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dxpdfskz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3luksmjgh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3syynbwda.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qcinjssx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gqgfvahs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3xvyfufhw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tphyiapp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vmltmcua.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbifrjhg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3etqxtfir.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wcmyfmxr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gnskrorj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ivplqydv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bftlzzim.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3plomkgih.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qbmqnqml.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bgwfstjy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rjqibfcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzcjikgb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3emeytmax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sakicjgv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3byquxson.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fxcrgbeg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxgkkfoz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjnedkfh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivcztkii.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrisgtfh.html


<!-- 参考信息 -->