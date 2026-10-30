代发 wailian999

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gbvqeyswg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/guwuibqim.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gsmjcmabh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gzvgiilax.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/guoffszjq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gpzgoaqmi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gijzkguto.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gtlawbsmq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gaqyippda.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggcfqnhkz.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gcuyogbjv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grfetkjtc.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gizmudzrj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/ggsdmquuh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjeemvpva.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gtikrelcw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gasprgmzg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gyyqbkbtn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gnkhltrem.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxqccuqru.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gggunrlkt.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gsynkwmnv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gwchoztoc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gutsgztwo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gsgdlodnn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gmxirluar.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/ggipfsajg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/ggljvwlhs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gpvftjspd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gmfbntkyn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gphagllmu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/ggbaacnbh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gabsmqhmj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gnmqbqsch.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gnabwqywj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gdyjrdfsk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gscecmjdz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqhfsojdh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gxnvydnve.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gsgrlvbhv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gyhwelohh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gwihjvmir.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gicgpmmcg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghkzygqsu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gslqhtpxd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gphimdahy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gbhwqribd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/ghfjpegcw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gibyjhoaj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gaumimbdt.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxrioxptp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwsbrlatr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/galhctzeh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gauochhdz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gcigygbrm.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpjqegzel.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqlfjgkgl.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gfcqlrcko.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqtoarcim.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggyofjqyr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcivntagv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzchmgnzq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdmlmouue.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghgbfwojw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfzbjsykk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggizzywxv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gqdjvussc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/geumxcnnq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gthwxasou.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnglbdgqu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/grkbbmwgr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gburxpmtq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gsxokjqni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gjqbubwrn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gcvlkybep.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gciwlrmtj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gllmrsyzz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gussayata.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gvgettted.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gfxlhxlww.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gfrzypbkh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gazxqcpal.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/ghkcwvnzl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/grqygbqbn.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gpusbdjwu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geigwbcvc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwxotytro.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gpqbbteyl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/ggbzuzkwp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjxgdhgcb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gqtjeqxrq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfvndicxo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/geihpesoj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/ghxughjaq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glpfdsidg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfmejmhla.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gilexegqr.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvikepdnl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gvkgmxsct.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gugympafw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcfynuoxm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjqzrucqq.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gcleygdjp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvclspsqd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbfhjszkk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzqspupok.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcfaebhob.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gyoecazbw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gpsgntsyh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/glfujwppr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gztxsecnu.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gijxujgon.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gydpgguqc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gapixaiil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gxddednjz.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gwhntipqb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gtmmjlgok.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gkukfrgna.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/geskuinph.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gylhlfaln.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxotumdio.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gxfhkvpub.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwplxesdp.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/geaaucdef.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/ghuxzfkmf.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gaawmgbqd.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxghahsyy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gkahcfoxn.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gfzbsmgwm.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/guogjagbj.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gscwboedk.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/geqfeqcoq.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/ggeyorrnl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gkpncuzoa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gsmrqbqyh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdrzbwfpf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/glfkxpulb.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gamoauszs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/giwdqbjnf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gxogtvdfq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/glyhyckwh.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gwrjupsep.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gfnowfsyh.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gqnlqnzxw.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggtfhpbeh.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/glopqkley.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/ganxfgwcv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/ghwjcsdwy.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glqfsbnol.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gidyoqjez.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gonlbudif.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gctflxydc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxzsnwxpp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gpyppftua.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gykkvnktz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpikddlxc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gtoijrznw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gghajmilp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/goevhfufu.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gmzygglrk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gahlwjfhk.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ghsuarxiw.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwcucyzfs.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjdauaekc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ggunnhocj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gzyvqjlgd.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/ggahhcncc.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gcezjlsys.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gjocxfhyi.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/goecyyqnq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbamobqti.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjgclmqpn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gshrjujei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gevvngjun.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/greajpnyc.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/glhirlubu.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gmssmxfnk.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gcuhvdtyd.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gdvlkesbh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gqxwbwtce.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxpgauntl.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gphjiyoeg.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gkbwarydw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gibsrtfrk.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gadwzsuyd.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gnnlhhwbh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gzbdhrsot.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gmjkowkcs.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gcfnjnmuh.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gcpbzbeyq.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gwtsrtzur.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/glkqktyzp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gmflkutuz.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/griblmiim.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/ghrhpqcxf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/ghcmtpcxh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gfwpdkeaq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gwkdmtlut.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gbbgrfehi.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/glezkbejq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gxzofpdhh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gaoajwajt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gazvunzvt.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gwmgabuwf.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gdatiosxr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gtnnvujpo.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grxsnurqr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/grreopzfu.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gszajuskp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gwfxckiji.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gzenszomf.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gnmrgulst.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gvoayoxmf.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gsmpkdgzc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gtaveywbt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqkyhvsum.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gkvyllzfe.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gnwvybruq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcailzbn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcyepxdja.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gllrdlqsp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gxwkwwptg.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gegnzpzso.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghbbvziwe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnlpbivjl.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gnktmmkpe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gghxnvjwi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkntwdenq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gouvtohip.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gdsdapjcz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gccqvcupi.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gezclfylr.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gqqsxfzdi.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gnvskymbx.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gduertgej.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gkvrewulk.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glitlkmwd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/guljzgdrc.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gprjibbed.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gwuuhaanf.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gxfkqbfqd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/guklifucu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/glhifhove.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gjrtrakcv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gqyrlkqmk.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbcqmjkjr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/ggaxniriv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/ggrbqhrnd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gpfgixlpw.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gmbpvnpvb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqazcxvvi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gaggjksli.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gfjakbrml.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxmzdllre.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gibywaset.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gbmoxtnnh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/golqnwnpn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbggdlorc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/ghrhqixav.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gllnofzvc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gbxakluxo.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gvpxgihbv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gltqfewtc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gchpbvkxa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gbkiozxhx.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gqikmnviv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gnvhzpium.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkxwhxjwe.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gdyiqskcl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gytagxmgi.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gssokgwls.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gfjpgpejz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/ggfuvziln.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gcqrepcmk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gfhurwzrk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gjnkguogp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/ghtqnhzlk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gyqcghmzt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gnabzloxm.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gmgitsxrb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gypwwgaft.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gwptopupn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gqiqrgdss.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grqymjmpv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqcnqyytx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gmaejetdz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gjjfthfcv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gurmbubut.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gwxibydsp.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gmpbxdivr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gktjwbgdm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gcfqzejly.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzxhqrvqa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gtdpudxlh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gkybyrqku.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gzaxhjadi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqqkcszkf.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gxsoibqbz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gijufmped.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gwgnwyhnj.sHtML


<!-- 参考信息 -->