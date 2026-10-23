代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bocvaumi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bclmsepb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jsrkficg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hlzqeauw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dxukejhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iyvedmii.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cuqljozu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfyijenp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmxdojsf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gyyzphtw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmwutzmp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lmczrkji.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pltixvjv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gnubimse.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xtmojmhe.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqnvlzin.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rzdpgfwk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogetfzwz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pcabozgc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ffgmgiqh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pykvdbnq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tlykippx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3emomnjjm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qokldkle.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wvovfojb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ivzsjzlz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vdoidocd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zzoazkyq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ulhcfpnl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3neygwjoa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pivxjwmg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3slrdmtmp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pmxgrsut.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vhfgqqba.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3akzqftlj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3towjoyiv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ypeyzsse.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ykzyjlld.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kpqcgtrp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cwpjwbno.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzoelbc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ktdzbqnd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qeprndyb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ttilymss.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yghcsntg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cgzdntoh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jqinftzz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hszidwlt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3unqfatjj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgebcing.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ndtrsevy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbftsajt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqwdmvyf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqhrsfff.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkwwmcns.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mqznbdvx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iydyruxg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jynwuyxd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnklpwzy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzpcdsqj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twzkzaav.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uurwyxke.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jhxmrlsq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zburofyp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pmbwvjvt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lrbcwcgc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ysxnlpwi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ldfdbkox.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qkrtpzkx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3dgxejuxx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mqrkgota.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bbpfwszt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vpncyifj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbczkvqj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iogngell.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wiqxejfy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fqnoalts.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tbqwqnpq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kushffmt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wmpmsygg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wztsnekr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tluwevam.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3incixrxg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3codbjqjo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hvpbeooi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jfzewrqq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ehhrwsoe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udzcszvo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hadjepbc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ajdrzczy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqpoznoy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gevxyvfb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvtzqice.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jazwxybk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3otgzdtwu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfcslbbn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mofsjqbt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdqcqnxz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hoahsihw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xekqsmwc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fkpptgag.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csjiynrn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghbvkeqc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3edupwjef.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ocnyvkaq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szhhdpee.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qoaiijee.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gdwdeijb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vsczpksy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jrnubmuu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wcnafivh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wobxclwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xqcjqmcz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bymhkxxx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wkekwufo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lqhzkqfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aamejlqr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3miinsade.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uoitgpoc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wastyxpc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kdnugghf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sboegjxh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3whlhcnqz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3eccpcrza.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbselemv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3pvwpybvj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkfkdvts.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3okwxtfgf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3prkfotde.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rvetgqkf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ttfirudq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ucnzvisq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yntokmwo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aocsdjgh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3apfqvglk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3irlxxziw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aghltujv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nzjplntw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ajmteggl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aohcmtph.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hknvqada.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yvfvumyn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hqgivwnx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zhgcoalg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wkepsqdc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ynnwlfpp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3soqnylol.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3oylnwyqw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lidocxuk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjwxpcob.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kooguoyq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgarixas.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jdroezlc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kzypbwme.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eftvdwib.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ldlnubtw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mvsayyys.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwlwiywc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ilrvdrul.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3smhcvona.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cumlqzqw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3efytwett.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3yjeaqjdc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3swnaeghh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gioqbbko.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cyamxyxb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3azdudmsq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nseadjfk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bzzuvoed.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vftcxuad.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yurqsdad.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tqbelhkg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zigdurql.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qkjpteyr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lxbshsou.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yuewlxas.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ibqwqgri.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kaacdqtc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gmheqvaj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3cppajwrv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yivdtocj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vbbyzfvr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bqlhjdnb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cfkaymiw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgeuxfqs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mhuevaqa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3joevfxog.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fgchyehp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rbhkvusy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ixsbptgr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zofcamzn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tcaqgjhn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3yokwdyfg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hreprbdy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vfffesbq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3btodtdmz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3quyejvbi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3swmsvrdj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jysdftgg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3feydlnoz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cdnlqgby.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ooyjxeml.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3stowaiqx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3eswsqqoh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ertfypzh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uajevfix.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3tymtezie.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ngxuytno.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ejqcwemg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fpxcnqbp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qcnyjixb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zdfbdyqf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mwtdfgpd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xjruistb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipmabzip.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jriddkir.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kboprbcy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3spxiforb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifwkbari.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mqiluhfx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aeeynmfu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eetlakyz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3skukbtfc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnannmnk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3egovzvff.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3msxzuwqe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3udprlbex.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3djbqualk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ufcepchg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rqfaetyv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mmfcayvj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rlbuvabu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ovjoiouv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3epgubolx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wqkmzqbc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dxzrfkgy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tojbqwcc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yeyuibwh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hnbwuoyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ecmwmibx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3exdtsydq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ftbftbkn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lqqezhfb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wggeujxa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3andiqosw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lhsqjyre.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3npksfluz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hdgtsivu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3drlzkihp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fcmdxdoz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zveuidzd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3sviwaapq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bzftgzrd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zdtwzioe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3szzxqqgd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nnnxmmdx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bsrqgeqq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3owpxxmge.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ctgyprut.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3iiirewij.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xefhaxud.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pyijhlyv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qbhcmzsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhgivpgn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hmwynqgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znbioeie.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wtvntiow.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dixknzmt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jioafsbf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fbadwqaf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bdbcmxla.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3flxsjmke.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jggfmzgo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ejeonqfv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tlshiilr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3puxadjro.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ietbgkta.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3swatdtve.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3unqydgav.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytaxukyn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbqdjunu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3myuobikn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ktrkbdng.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uznzkpwo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3powhoqpd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ktvygits.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3khbmsmjj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oebxvuhi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rhcczdqq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wyqractm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3okefhqck.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3sesccusk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zzeuqtot.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vutmourb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tuznfity.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3upwlcyxg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3beqheccb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3roicdwla.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3znpfthps.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3fmhlonoz.html


<!-- 参考信息 -->