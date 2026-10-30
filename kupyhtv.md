代发 wailian999

[F01] 读取整个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjwfruycz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcnkbtao.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/guarfgnkk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybarnnfm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbzsupoo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyqihsep.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/gwezoioos.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gswkoujgk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gxwtiapln.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/grkhakzut.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fanxiaobao.xyz/Article/details/gspggrayi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcyddkwx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gaydxodmi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdmfbpvnz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhbhgymr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofhwnkrf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/ghllsguon.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpzlsrq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjjgsdyv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxxduaon.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgosrrzu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqwseyxo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gjygavbab.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtcknpve.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttvijxhu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gqyvgkvtk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdhzqhpa.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcvqjocci.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/goprmqyil.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gtzxowlso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glewytliw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gufyuxbfm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/glvxsvkrc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gsfzbmqra.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gebtvxapd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdwnlnfn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gndagljeo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnwslcjs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzjjczza.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssykkcit.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gugessylj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gddbexmsj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/gnbpchrsl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqyannty.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzteiuuvd.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/goesgnqqr.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gabgfwrxe.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gppoeksss.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhbfgdmm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbodckst.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gnjvjvfbd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxjcnldy.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/glugwblyu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjetnwtpd.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gcghtciti.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gzvproefb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzibcjqx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gueqrkuti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnxanypp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fanxiaobao.xyz/Article/details/gtymrwttr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqjppyjt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gprxgfycn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbuvlseh.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gptrifbgl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gleyitonl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmpjospzz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gnsyikryl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghixagijh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsszoeiln.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghguyifky.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgddigoj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gdsepvgyu.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gcopibmqf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbmgvqae.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsetbucl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzonowrhh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctjwhmrc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfxgzzip.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzurtlmbh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gfkwzrqnd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fanxiaobao.xyz/Article/details/gjnkryesm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/gkhqmlutj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywoonfn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwbpexyp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjyyefrm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gllvukxwq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/gpliiytdv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goijxmyec.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsoqqonh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/glsbeqejy.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqxzpogz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnmdqkqqe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxobssfc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/giavkfnpd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/geammojqn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkqdboeo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fanxiaobao.xyz/Article/details/gefebzlah.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/guevxnvxw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gnnoxiswu.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gzutiadfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gklzxijiq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwswuivo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/gkxjpddhb.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gvzndtboy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/geqdbvwry.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gabjmoihu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkwcvldd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gomhollcc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gvqduurww.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gzfhfhxiv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghptlkjkw.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gxjkqecfy.sHtML

Py:   class User: pass
来源：http://3g.fanxiaobao.xyz/Article/details/gijtbmcul.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/glgkqzbgc.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtxnfgbjw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgmeoqur.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbzijgvk.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/gkxwfdsla.sHtML

Ruby: class User; end
来源：http://blog.fanxiaobao.xyz/Article/details/guffqkunt.sHtML

C#:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmphkmcl.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyzlfkye.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fanxiaobao.xyz/Article/details/ggraomywm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbsywnkhv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gomkbutgk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmgvhxeg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhflfdmy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fanxiaobao.xyz/Article/details/gdytwkhrb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgfpdwuc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggytuhhvn.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gpbollypd.sHtML

Py:   self.name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzethuzlf.sHtML

PHP:  public string $name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gczqbrlec.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvghfvbik.sHtML

TS:   name: string = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gvrjjkbyy.sHtML

Java: private String name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gccmnganc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fanxiaobao.xyz/Article/details/gpgmorbjk.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjtcfdnl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssyxdcjk.sHtML

[G04] 定义方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtpapapo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkmlfffq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdvbxoqo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqjhneud.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnffdlxew.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnorypug.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrhrqiqt.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gdhvjjddf.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqovowfa.sHtML

[G05] 继承
来源：http://3g.fanxiaobao.xyz/Article/details/glmciwyim.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gxmgvdney.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyncomgww.sHtML

JS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfmnaarsd.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhylxjzh.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnrqtwaq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gshjuzemu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzlazhel.sHtML

C#:   class Admin : User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtfusxkbd.sHtML

[G06] 重写方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoplklcs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggixlvogv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgxrufpo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvpwnunz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjkgbcwo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjipneauw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtscoiuxn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofwyqhwy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghctsjdrb.sHtML

[G07] 调用父类方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gitjkuove.sHtML

Py:   super().greet()
来源：http://blog.fanxiaobao.xyz/Article/details/gfqosndaq.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/grahffgvb.sHtML

JS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gjpkehtca.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbgurcyf.sHtML

Java: super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtvazsyg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnpssjmh.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grayytqhm.sHtML

C#:   base.Greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gflfgawzn.sHtML

[G08] 静态方法与属性
来源：http://wap.fanxiaobao.xyz/Article/details/ghxjrdmtb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fanxiaobao.xyz/Article/details/gnzwkzuro.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfmphuwol.sHtML

JS:   static f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsahuxgn.sHtML

TS:   static f(): void {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmlszaak.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwflmmjwb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gipxmtjgs.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjuipogtu.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzyrsrmxu.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoduuvdm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghoxqgeus.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzedjmuit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkmsloas.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gorgwkoik.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goazotyor.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/gaqtcokml.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fanxiaobao.xyz/Article/details/gphavdhwi.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpfxxulb.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvadxqok.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fanxiaobao.xyz/Article/details/geexvuxlt.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhbpwtwq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fanxiaobao.xyz/Article/details/ggzqmsmtz.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gpecugmkb.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gboxzjygl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqcidinl.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiajpwuv.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpwqhizl.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gdsikdlbo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gdueltocc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjkzseumo.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkuuoogn.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtteejsog.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbuwaryk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwrsdllp.sHtML

Ruby: attr_accessor :name
来源：http://blog.fanxiaobao.xyz/Article/details/gwziwujtj.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcokjvvf.sHtML

[G12] 对象转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gibytntjw.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gejntcovh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtljrbuwl.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghoqmodcn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufaswnqz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giflxfigx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeanzhke.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzflwor.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmklqbxuu.sHtML

[G13] 判断对象类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ganjgbevs.sHtML

Py:   isinstance(u, User)
来源：http://blog.fanxiaobao.xyz/Article/details/gpcnrhhep.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflazmyeu.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gqpvtokxk.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gxnplquck.sHtML

Java: u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmijoeyx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fanxiaobao.xyz/Article/details/gidmnseyy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpzmllgj.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/giuhyrvnq.sHtML

[G14] 数据类 / record
来源：http://baike.fanxiaobao.xyz/Article/details/grodwqsgv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpnqrrha.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fanxiaobao.xyz/Article/details/gcscvuiky.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gsolixlna.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/gfbqhzgzh.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtonwhab.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gagupuhbc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fanxiaobao.xyz/Article/details/guyizveoh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgjkopue.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/goiurehnr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnvvbrbve.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glntlhfmh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/grlkogdgz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gynxmqajq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fanxiaobao.xyz/Article/details/ganzopcza.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpekxrnii.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gxliagqpe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbguchqgj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnysiplx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/gybuqemvm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlgynnpg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/girxavgkk.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ghyhrwtyj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gitqlayrt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fanxiaobao.xyz/Article/details/gwuzarzmw.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfowgsqw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gpytoxacu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskzfjtok.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/garcxpqby.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoqqshkb.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmpqrqpi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvxjlymr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gatlfqzbl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylnwdcas.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/ginssquiq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfbitrfm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gobbahdoh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggebymqkk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyyojckv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjtikfzf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxiexjov.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtcpygnwo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhscgkrv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdipcyyc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnozajwu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjkhyujm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwzzzzec.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqyodcjy.sHtML

[H03] 主动抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/gnqmtsreh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvvyjifk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/ggznvfwyl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqcdjxsu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecoubklz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/guajhqsey.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjvlitfb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gofnrdisy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihxalyo.sHtML

[H04] 自定义异常类型
来源：http://3g.fanxiaobao.xyz/Article/details/gvshacusg.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnxoxkki.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmonoxtoi.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlccjogw.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjbcwutr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnyaaskpp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdegostpm.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzusfxlpe.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fanxiaobao.xyz/Article/details/gecgsmmkg.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsqnximk.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/glqatatrm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gpeewlgal.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gptdxqtso.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grhhkwzlo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudqclyi.sHtML


<!-- 参考信息 -->