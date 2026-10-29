代发 wailian999

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gixvvbqqe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gyzcnuuls.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdhsnmiyf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/grugwvzwz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gssawsefo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gvdwwaxiu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gsrluqllf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grgpkoynd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmhfgiiph.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gsyqfcrub.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gmzaninta.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/grkzomqgg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ghsfnyivs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gmwqcazcz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gopkgpnds.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gmbumhuuc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gxskpkkoz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/ghsxfvimk.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gkzoigzld.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gqcdxnycz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gazttuglr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/griiyjvrw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmnugykt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gtapjpweg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/ggcquegqu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/ghqszonge.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbkwoabzd.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gtjmcdzev.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gjezadzwh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gdxxgpskj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvishhcnd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gegpubwnn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gbuxynhbl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gssmpcfhk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/ghpaolamj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/grmynhxsx.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gflpksrbn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gzpnyawnk.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfnhcjgsg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmopgnfdp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtbumuiyl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ghaffbbse.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gjxkxmfeg.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqtiqfffl.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsgkxcsnj.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gthqvkigb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grlultpms.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkxrbdzis.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsddpxjyd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmwrukiyc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gntsgdhds.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/giyjldhde.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbdeckifc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkxmdygln.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/guxkrtmoc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gicqveqyi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gzptmnbbl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gdgmgroqk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gmolrmtyo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gnjkotfha.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gnmwvnuuk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gmpdjupde.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gqecaohqq.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gtvbeuzpw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gokxhbwzc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gmelgkjhj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gpijhysqo.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gpkxvhgar.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gclcglgmp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gwmbrceie.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gruesugng.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmdqfyysh.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/geclcddsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/goesfmful.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxervgqzx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gqervxkpu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqzwdbuln.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gdphisqev.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gadurcjiw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbynujjbd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gzgiwmbso.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gmytdsmoj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdytgwedc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gikbwdzry.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glfovyzrx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gaphayrqh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gjosbilol.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grgvhaqnb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gftfnbpkl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdyvwfcgl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gxkithixk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggoilpaza.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcfolttog.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqduqoyip.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/grqwdtcaa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxiywnryn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/ggrqrdhui.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnhwcbwbm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gtngftdnt.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gjfxblyau.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gqnxolaji.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gawrmcmsq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/givgumwgy.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gscdmsppy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/glsciscck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gqmqrjrca.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gxwtqxuiz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gyqjjkyvz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geksbngbz.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gndsuewed.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzjdljwbl.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gckrokrbe.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gngheukuh.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gtsexhmap.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gdglpixwc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gaafkxavu.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/grsgbbeya.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/grkmoqqzl.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/ghozdsuxz.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqagcvmre.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/golgjavuc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/glzdkyurw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gsqzmjylg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnceobwwg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnwoceveg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gpiebxyyg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gnkcfjqnu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gpgvjbmwu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gszxznwio.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gctcbrwnr.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/ghfeipvtj.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gplujihqi.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gblkdothi.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gvzcpihvz.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gdbvvqtpd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gjfrunmci.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/geshwlfuv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/glruuusjn.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gwjxejnmq.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gxoedgzxb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gvqtxjbpp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/giuhskwfe.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gehykizgn.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gidfmwwex.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghnvehfnb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gzwnmwzjv.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gafwelbbh.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gjyztblxj.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gtlkuspij.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmpgctmka.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmgtixywx.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/grdjqnfur.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/geitixalj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gcqlbnfhh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwhajolbn.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gdcikmptc.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gybexyqup.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gqxwfthhe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxboxsyxd.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/goybapiri.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/giwbjrsnv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gedmemicb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/ggfphzcqt.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gxqnqegfq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gvwjljspo.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/getaiswms.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/grefwdynw.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gmkmnqyxy.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gyojgqrpd.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gugkrmruq.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gaidbwetc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gqwjyrcep.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gipyycmna.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/geulofjpz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gtztkxqfj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/giaiqouxf.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gfzthfwqk.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/ghuzdwtdn.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/goespgckc.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gkmxicamx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gpttvgmhe.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gaynjsnxk.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gbbnaqwmc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gfbzqaxjk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gmdvpwtxd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/ginsevwnl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/ghrujwpeg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gaamixubd.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gmrmaqags.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gxlrpyvwv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/glxfpodwi.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/geyjhybhg.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gtnkyezfm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gnsplrgci.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gzrkxjaqw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/glowykkys.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzcqdqtgs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/greqlgrwg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gndcyjzii.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gkwkwcsvq.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/glpjeknlm.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gstowvqur.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/grmgxjetc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxdwluybr.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/grdsxbakx.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gkbnnxgwc.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gtojacgzq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gnfhqlkao.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gjumlqxrj.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/ggfaohxtc.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gsdznyojo.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gntriylzj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/geunqzejx.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ghvmiawpx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gplodglds.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gekccqdfp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ghrqgaapw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gzfoxcihe.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gbtyjpqrp.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gvwdwntuv.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gmyhdfaap.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gzzdsggxz.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gyqjhrnqe.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwjsdkkck.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gsldgxvln.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gyqaswoct.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gqhacllwp.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gyjijkpog.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gbyqruyop.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gyqxeugwf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gvpzrfqyw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gvhuedcnx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gfbmtzbcd.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gvydmyaag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/goqwpxqqy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gmkecpygn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gjcvktugf.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/ggkevwzpv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gtiwjanvt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gtzcknuqp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gwlakvzhb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gnwqmfdlf.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gzlcvmowu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/guezcwout.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/glauklizc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gdnbzfjtm.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gcaujjrde.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/ggvzamegh.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gvdwsxzbh.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gvshemmag.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gwoqairhi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gplgdduxa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gmpncgmfn.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gshribdsr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gupmolaio.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxqlelvlf.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gevgcntey.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvliocwyi.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gxjwdiofl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gougqwbds.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gfiqmomfs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gjiwhmlfs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gimqeeqdb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gvlqrhnfy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gcvwqijkl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gunajrtml.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gjnzhancc.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gpqjsiadh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gktulxopm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjracgxae.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtpszdgkc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvisvjuik.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gswiytdzq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gpjigdyyi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gxbrnaihd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gnipfgphd.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gfjuisdtj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gqwvrhqfs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ghdwsahml.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gzlilyndj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grpcwxeos.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ginylfsvp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gmauereht.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gfiydeuig.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gujgdustw.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gskxsmnvl.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gggswibtx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gwannrevx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gdkterplg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gambtwpmi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gnnxkoyll.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gilefctce.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gvdvhufzd.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/geriaecho.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gzirzrtkv.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gxjpknnit.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/growclogx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/ggxcrvemg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gjpumzgcc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpiwvihfb.sHtML


<!-- 参考信息 -->