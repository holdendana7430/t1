代发 wailian999

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gtlimpiao.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/ghrjzxung.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gwweutrxd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gdfpziplb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gffoblrqf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gztxjjldz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/ggtmojezm.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gfaogsfos.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/goilludhv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdkjwiwxc.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gfvwftuav.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glppjqdee.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/guibirhej.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gqzsrewqf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcuqikamr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gchtklsim.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxfazlzfd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqcqqpbjv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gotzvumcq.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gffcwkoiq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxpganlxx.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gexoambvs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gzravcwtv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gtcbcxdci.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gycpnyqfk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gorhmrhui.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/geupvqxwx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gjxlyrwpq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gfdwlojoz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gvyfpaegs.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gdahbhlgi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gjknvhjjh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gaqvqjtbh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gmnwdtjkj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjqaytmuy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gtdfvetev.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gigmlhxbz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gnfgkwkon.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gtqqzwjsn.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gbrobwgml.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvaypkbgk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gxtxvtqoq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gfvgouhad.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gyswteido.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gndrmwaux.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxxultsdo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gedtornmy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gldoywqgj.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gfotifulx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gomjxwwkp.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsrjlfuvq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gshjehlnw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfhzdvjok.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gjvlrhlwg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gjoklydgw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/glilipioe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghyhjcwvs.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggzwdadzm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvnngnspf.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gyayttwch.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gexnrsicj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzzdktvbf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gbwnjyosc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbvmtlagt.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtcnyernt.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqvfdckne.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gedzixjdb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gutqqodfd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gszsgxtgf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/grdhttntm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gqgkzxsld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/ggspltnmk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gtargvgey.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gstzrhzpo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gazncjnsc.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gmlmsnjnj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gpxvazibt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gzaxaaeaz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gsvilrmsf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gbfzkgdhv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/geayfmrzi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbaoyeavp.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvgdxgrlz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gopgilynv.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gvmrpfrdj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaqdzjkrh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggemrhqfa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gcepqsnks.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gvlxflkaa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gdzkphbhp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/guoovwujc.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjdwbwkyu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gpqhcphik.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gztjrwwxk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/grvqmcaym.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/genmshkcs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmmjqzjua.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggrhiefle.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gwzuxfddm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gearrwdlz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gktdjvxmi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gylsknyzd.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/ghcxohsyh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gesgumkuc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwfnqaoth.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gnkkgaejp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/guccvxdws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gerkpnrdc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gzqodempc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gutzpuoek.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/glsogpiqa.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gvodnovrc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gkdtndqeo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/ggygloosk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gmwgkzleb.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gbpkjfyvu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/ghoznixtd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gpmmwdzum.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gjkqfgdhe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gcisodfxx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxfnerbrg.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gwhoiqhnd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grgodxlrg.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gpvlwysku.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gkhkegnne.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/ghrafbjdf.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/guqxrtvlp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gzmexztnt.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gffmjwjtm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gsvzzlhgc.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/ggetqsvsu.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/graamdltp.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/ghdhtqysu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gkyzboxjf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpiyrembe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gvckucbsw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gggqudwlv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gnphyftxm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gzhdztzbo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gsdicjfvp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gnnwbqpvv.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gywkvexke.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gkmtwcnow.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gtvsltsvy.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnzqonsls.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gxjsorply.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gtzymwdqz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gsmxlumdy.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gfgjabyrb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gwkxdnniz.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gigfslilf.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gabkiwptt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gwcguieal.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gzcnwhnqw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfjrazhgf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gqggkirnn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gceoiskzy.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gubjtwfpp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/goulwloml.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gcoojoecp.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gvaljjgfn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvpselzlk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gbnhmkupe.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gukrtyixe.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcgbjkqzx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gnlagstiu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gvpbgoaxa.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gisqxdxrz.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gdgqdrosg.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/grbrgpsvk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/goblieodl.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gizfaiglr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdnolqkab.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ghyqurzdv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/geizptfpa.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gchwrymii.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gufvxvnbh.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gdwqanfvu.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/ggytszjhd.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/ghunjykuc.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gakmorofj.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/guddngxyh.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwnmwcitj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/goqvpofcq.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gozcdklsi.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gngvtvase.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gtxrudrla.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gybexuwbr.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gecdlulni.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gxlsckttv.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcnzxsvek.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gnhaflnou.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/goknlfldh.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gxvkkituz.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gozdljpkm.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gvdzjluus.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gfpjjxcfp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/guvdbknxb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gvttubriy.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gmwvyiazg.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gtfgtgubs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gtdbkimrl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/ghyokuztn.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/glujuvbdg.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gwrjkbsiv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/geqrqxtng.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gujxmlgaw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/grzccyqte.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkxqrxfiu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gdyxbgzna.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gctksqupf.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gageujcsq.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/guvgubiwy.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gykufnmth.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gykktexon.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gcrkskgxl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/glpfbgwyx.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gejwogkus.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gshiwjnjn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gnlokxjiw.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/givjyptzh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gecfkrnaa.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gfpjfrhzg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gymtrddcy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpiczxrin.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ggmeqxgoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxeindqcr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gxpbmthpa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gjbdieetp.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gtkkyfcuy.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gpanndyej.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gfiipdlpc.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvotehaol.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gwawzkzvu.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/girepvuol.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gpoilamnt.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gjpzpyphz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gfmfsujyf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gltruditi.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/ggblsgyyr.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gockahpuf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gicbwtmiy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gjhclcbqa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gklogvini.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gyhkifkrx.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gpfvtwqdb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gbbehkmuo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gamqtdyfx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gwtqelbiy.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gdsocxqan.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gwlylkwbu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gassfvggj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gqlkiyvhv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gqnzgcngd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gsoeejeop.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gkhliycdl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gilzhclny.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/glptangwk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gmzdjbpli.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gqchttxcl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gvxsqqwkn.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ghbwykwly.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/grkrooppz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gzqyautme.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gkgqdbzfl.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gzpuzyghj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gfbgguxpe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghcqziukw.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/ghqunngau.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glbebbyaf.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gwroyxmga.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gniltftui.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gaqnmiraa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/giqzpoyxs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grcsnzixe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gcoduihai.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gkjftbipc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gwtoadnfp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gcphonnce.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gpiwlvbxj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/glcvdcclx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gtaxwcbsu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzwsnsrys.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxqvrrsdn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqekvatme.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gaypnqegt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gshwgtpmi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmdvqnsbk.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gbjupuvcf.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/guupfrmla.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gueamyvnf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gpwkgbjnj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gzriruvwd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/giuqdayap.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gsapfpcim.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gttyrbcbk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqplvuezv.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gxyehprbz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/glnkkferh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gojghqqtm.sHtML


<!-- 参考信息 -->