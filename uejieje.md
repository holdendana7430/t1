代发 wailian999

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/ghlbwexcs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/guprtmtjh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwoodcqrv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/ghwwrxcar.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/guslrgeac.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkwfijyde.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgskfut.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyvgxvonk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdmvsjbjb.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gjscgxnui.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gwiqqssru.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gpffozfzx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gvvtxcddj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gadxemdae.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gyqfzlzfm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gdljrmdti.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/glpcxodxm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gfpowupdz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gwkomuwwp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gzbwczkth.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/glnrqimom.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gzhxwwvoi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gczbbakyh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gigdlfozf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gajabjolz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gkuyqfbel.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gmadrsbac.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gnahuqjfv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gptitfyrq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gfipaoahp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gejndkese.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/giylngjro.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gbndtpgex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/ghmjneilk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gmixfzdor.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gzbodudpx.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gtemqzgbg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gfjwozynq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghhftldiu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggjfwncnk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gggqnmwoo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gpncwgffq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gnmljtbkw.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpopzhyjn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glmrqffdc.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gcegatfjm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggvgfxyqr.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmtepzbuw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtlqzvoze.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqpeorso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxhhdyyhv.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfimzjewc.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcfnbjuse.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdvdysepj.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gzgdhehiq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gafkyhxls.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ganjdsqbc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gpwclgsur.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/goyokesvo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gotgacufp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gfmyadsho.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gsuqsmmhq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gfzdutndd.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/goznobhac.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/glnieexlt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gzdrkhgtb.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/ggoudajev.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/grohnqvse.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/grtzjsmks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/glnrafbie.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/ggavxccqs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gwwnopsvh.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gzhimklqr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gggaheanu.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gusopbnin.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gdaofihkz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gimlapekh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ggotdusxc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/grqcoggpl.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqzyxlpta.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gdvrmevpw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gcxzosrsg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvdjawhis.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gflqesxbp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gheppvzox.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnkhiaeyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/glewxkmtv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnexjxfen.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyxqgigtk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glezndumf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gsuznvbxk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbxjhzyuz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/graqyhvej.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gllaekhjq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gyzdqfbop.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gplwixjgf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/grpxsalxj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gallcnlab.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gqzkadzjo.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gnosqvenv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gclaznxbq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gevzdlfpz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/goxyclkfd.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/ghxaiwuyv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gbeaxmckt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gpqsicwni.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gvdmdhzht.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gsispheiw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzcggznjw.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gawcxxgoz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxlbrznmx.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gdhjjktnc.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gonmkofgk.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwrmmykhz.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gakflzdkn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gmcwmjxua.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gqdudfscr.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gwlcnfniq.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gljvbsejs.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzgoulzhj.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gazzorcxp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/guqaokhuv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/guapepdtc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gvvcfgvxp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gilccakgg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gdncsiwhn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gtiyowfyi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gqulwxemi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvdoqnejt.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gzwteepyw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ghqvftvom.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gpoygknpn.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gujpdekdx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggqhpkwek.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/glsulvaex.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gemtreyni.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gaqnxomtd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/guywdziau.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gtodnqbhv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gdwtyaffe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkhhimmvz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/glqggiunz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goluwkwcz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkaizkztc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gljhwtkzj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gfjkuwvra.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gjcsitlzx.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gfkdipsfe.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gdgtlysng.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/grsguqpot.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gifvclsjy.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbazbuljt.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqpvcupju.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gcqgbrhfd.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gcrimobmd.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gcccrsowu.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gliivlzzi.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gllmlpnio.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggfskxqah.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvorbcewa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gywmuemgc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gspryunry.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gsvwrsmdw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gtugcsueo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gwgrrbfzh.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gradsntjc.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/guvtinptx.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gimnvpkny.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdwogzgij.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gmmklidnc.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/glmtxhkyw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gjjgtbcxv.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gskykpjuc.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbysgbbtl.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/godjaufom.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/ggenpuvdq.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gczdsymay.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gpcanumqv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gxrvfulmq.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gfumfyjnq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gyfbwirti.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gtzgujghc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/ggjdcafcb.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/guaumaiwj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gmfjylysr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gjwmziryf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gtbslgzyf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gdpsjhzbq.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gtgyiyadu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/ggimmajbp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gdcgykdnu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gfzaberij.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/girlteqtm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/goiferzpx.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/glvgecsjr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gwvdyhbre.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ghmeqgurt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/goebnahyv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gotdloxot.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsjzheman.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gpkbathxt.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gmghwmbex.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gdfnafybk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gwcdxzhgw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gjuyguyiu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gfjsvfxgs.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gyjzoxalh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gjajjyhtx.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gszkqsvij.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gevsshejo.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/getmdmfia.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ghhqlfrsu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gzvzmbmko.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmfcwperr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbymhohrq.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gfquwgaov.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gltcaijcs.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gsbvpkrth.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gydtqovzd.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gfvetljkb.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gdkpkjitz.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gqoqmneji.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxrjhavai.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ghwtzyeox.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gcxdacgzy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gthluygdf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gnyruliku.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gpbrnqbsl.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gjbwjdugm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gxsitdxyh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gigvnoyji.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gbphimaxj.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gzajzkfcu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/glzhwragd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gulwqbwwv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gkmsnrdcw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gyrxgblaf.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gmetfxopt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gaebnchmn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gzyerskuj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gmojtkfob.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvfuiqhba.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/geustuywj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/grdnpfqtz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gunugxwuv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gkqaibolp.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gxzknojwj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gunjatcnj.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/glxtypdhe.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/geyzsgxbk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gniebsmbt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gmvejsrql.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gaaxoyzyj.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gutqvqqbs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gughqyfen.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpxuuqhgd.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gloylylbk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gldbwxwwx.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gaxwylfyw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gptqvktgr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gtbvbzpqh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gavuzkfvg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gyfuocnge.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gdomcskgt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gvpamsjjj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gamjdrnyr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gkeoyqzeu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/grhnezpok.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gugvdgkwo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gudkxhski.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gktoxjxme.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gjverksmu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gjvbvwjlx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gplimsgvm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gcosngpqo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfejyhyfp.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gvkdxszit.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gpiygizww.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grkplnpuh.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gzlcdkamq.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gvbbhotfo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gdvbwthrr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gqgrosuhy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/guyzcvsrk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gojbvgkjl.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/ghjqsxadt.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gbjhdjcpa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gomgkmoyh.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gtgrhdukq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gpmeksqgs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gnyvzthrg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gedapozet.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gfqzcrody.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/ggbtsuqto.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gaezttvdv.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/giedaxqhd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gzngihuro.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gdmybekcu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkcstcvve.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gohdjokyi.sHtML


<!-- 参考信息 -->