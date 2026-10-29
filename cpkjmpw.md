代发 wailian999

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gcxgiyyjn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gpwnysryo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guszbtgcs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gvgytkyzd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gczkmkehs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gubhmnmcy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gxluslurv.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzdxaoqzw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkifswaed.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/ggglckaxj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/grifsnlvb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gyerzvdiy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gfeposjuy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/glkjmyeus.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfsrqhnf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gzedvklrj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gvblmnkij.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gumjupoxl.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gvbtabhhm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gzlizdzue.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtrcpgbqx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grvyyapco.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gxtopmsuk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gwmntwaht.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gabllfcud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gofbskdvr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gfmizsqyl.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/giuncmcod.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtozyzpfj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gzoadxwxr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gotaeorfk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gobsmnpxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gttskmlaq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gxtlezdow.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gbvkigboy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/glvlemtpg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gsdkaqtil.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/ggeeqojtb.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdbykyrcj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmnahmxf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvoaejlqk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gmdrfgold.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gnawgvutl.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtrjxytgt.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/givsolnko.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gwobrijkz.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/goxnlwxyj.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwsmaliwk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqarzkwsq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdycwocvn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gikwznhgx.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvmonhijn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/girkjohhi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gupvbuyss.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gcsgrmttu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcmupeiss.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gcwcjhhuy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gwhwbrujb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/ggejpoqcj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gnpjczdkh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gcplacdwd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gbusjwntb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ggsipjsai.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gvqusmsiw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gyrdmwgtx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gqurxzsyc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvsvzjjla.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjrjxfybs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gzwzlioni.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvjhmtkwz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gnozotzdm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gqdqrsxez.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gxlmlpwbp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggqusjjvb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glgbwcibb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gjnrlsxod.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gczbilvwk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gsmnvvnzv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gqcfjvoas.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbkqxjbtv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gceweucwc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gpenpeaym.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gattftsog.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzbbrmngo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glduffzjd.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxktzmnhr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gzaoldorc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggpmifwno.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gvdbbgocw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxeqlfxkl.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gfysyqrjd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqtgwcfta.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gddfjrhld.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdbxoetjt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvysjjmne.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gdyfpawgs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gerzfrggf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gxdszfuea.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gcetgqgno.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/glpazhdyj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gbnbbkpby.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gszofgxkz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gcooinvau.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gtjyxeiyz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gvlxfmmih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gnvrhtwbv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gcpkktyjp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gcbvhjrvt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghltqgobj.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gmxuednpc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqaxmyrsk.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gohmtbfwp.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gornmlryv.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/grzbkcbso.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqumclsue.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gfsopaonw.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gegdjrkzj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gykzxoism.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/glpmnzphv.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gmxhxrjzm.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gympuphog.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gjlyqlins.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcegqiopu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gtnxwtivn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gczajnwdu.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkwyaqvyi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gwkqtiusy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gdrowvihh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjrparogp.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gzaejlain.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gqeomdklo.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gbhbzasyg.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gjvpfwkcv.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/grlaldkgs.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gzlphelkt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gwxnqlecg.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gazcqczuj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gutcmbylm.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gpbzqnsjj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gvbcayloa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxvppopxr.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gouopqzuf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjnmshweu.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gtghigbbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gzrjxxywr.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gjvyyqnoh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gxihfpdpa.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gvluwkjrb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gckeeeyxg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpnuxfrtj.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gimfsxdse.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfbonrmsw.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gkdljfjft.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/grhkzcosz.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gxtmbozbe.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/ghffoetzs.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gqtljfgid.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gpayqrpzc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gutnhmqyd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gbuakhdik.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gypfxmhrz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gzdpyyucc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gvdowtxyb.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gftkvuark.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gzbdhfiue.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gvxzsrryo.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gyxzupxbk.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gjswxtrci.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbuxmmdlb.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gmzmimmki.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gpesynjcq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gdntamxek.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/grzxnvejo.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gwnufpnvv.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gxblcjsgr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gdujnbabf.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gnrfcahbl.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gkkhwuhrp.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gmpcnqkql.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/guxsqqpdn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gqpnaqilz.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gkvzpuxxf.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gkfkwsdvb.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gyvlcdtwx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gizthpqkz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gpfrhmsrq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/ggmlmnwhu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gqfkywfol.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/glvcpjfem.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gbcbervyh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gubvxvhxy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/ggmgditeo.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gxsowejiu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/ggxvwlxyf.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/glpmkrxej.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gsubvxzsm.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gajhmgmko.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gfizktorj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gtfinlqob.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gcyzhgcjn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gpenrlpbe.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gsbabqart.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gknhvlkrt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfyyiwtb.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gsegezokp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gztfmbcdl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqynvfbvb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gxddcdliv.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gvfxoonga.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/giceeirzv.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gyokmphtv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gjkgkssxf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvqiwqibq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzhphcrjm.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqjrghkha.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gucppzloq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxcbpznyx.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glmjmdryb.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/grdovwvqu.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/giodjcskk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/ggolbdnjw.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glptvczai.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gavdiqlrv.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gtosmthaq.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gexonuzop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gynrbcfrk.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gtxqanzio.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gwfudutqc.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/grduiwnug.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/ghwtwevjw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gsubmptqk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gyuzpmtlp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gmimqlbsm.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gjbvhpfys.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gqlyelkol.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/ghzwfvjpb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gmmpnmxbw.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gxvncnsuy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gstfyklmc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gsjmbobsa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gdpzpgsyn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gjuyumshi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gdpnrmhkv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gpvklosen.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gqbavdkjn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gwqgyxiyp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gotogoutx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gcqvpuuae.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/guygifgfr.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gmhnegfgy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gydibncbk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gjblaxfsh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gelugcuhw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gvjampnok.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gpxekeigu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfjejwexn.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gzgbqmijm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsawsjedv.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gyexhpjsa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gmhnblytp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/glghiwhoy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gkhndvlog.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gtqepbdzg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gemtdbsue.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/ghtvoaivu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gwhbyvgoq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gryiysvyz.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghyxeoqor.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gwmpenpns.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjdtyoqtz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gutrcolpu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gbyrlatgf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqrzlldgy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gqkygnlrt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gxyzcgqvf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdkztzkxp.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/ggkiebrce.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/ggqbtenex.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gehkjftmr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gkbfcxdnu.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/goftiiogu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmsopahfo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gfhmiffeg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/ghbdhfxat.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gcbekdrtu.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gulyhgljk.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gsbxagrpi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gflwgwlrv.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gatnavxsr.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gfbczlicq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/grtmbhvwd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gsiuezfro.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/ghiwcxqss.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gunoddovr.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/guvsryvha.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gndudvcgd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/guhdiqkby.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gqtocwylq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbkhnlyso.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gvhwbcker.sHtML


<!-- 参考信息 -->