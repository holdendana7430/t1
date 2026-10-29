代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzuwjnsxa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gvmzabkzc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gtfbzmdja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsvcjpbhm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gmbtjecdp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gaoqkzelk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gyhdfkwtq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gjdxggnhw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gavjtnint.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gbyxpuumr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gldzmkskg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gnzqzoweu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gxydhsahx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geohewbql.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gimriougy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpqtvpzis.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gdefblwxx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gfnutcyvs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gogfeoziy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gxgiioyyu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggmvcmobb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grlclnsdp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gzgloctwb.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfaqsxcub.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbwjixdrk.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gddfbinvz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/ggmdzonbm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/glwnnlctk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdxtdqnzp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/goektelcy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/ggzrvohnc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gsegxkltf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/ggcjkwnzm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gsoeadotv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gielmkelx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gmgumccwd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gaovwpnib.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gdfmxtbks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gifjfbefm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/giozmayjb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/grhkdmbru.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/giqsckzxa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggavxqefs.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gieroxvxe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gsniftwxz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gshohjrfn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/godjtxtia.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gxbsepecb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gmfqzuqvs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmwzpbmob.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gvxczpiva.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gobsefrob.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gdhwkvbiq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gvyilcxjn.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzrzvlbkv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxjxfufxf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxcyymsso.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gxxdbdgdf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gwgiyfxjc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gazfxkjxy.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwzyykjdn.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gcqbcwwnu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpttnqlni.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxqdoebwo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxykpvsjh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxpajgqyg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/goygwmaaz.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtmqkcolw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grkdjxyyq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvzyhnxri.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gmsfslpcn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gmynufmck.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gwpifetxe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gyhsqyquj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/grxpcdlmr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/glitdqksf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gvvefkzue.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gusvyszlb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gwluuiuqf.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gtwdfijuk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gmcstcwwc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gjbdhcmey.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwqmynaco.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gnyigrpob.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gvawzeoyf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdijycofl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gijtewutu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gzuihupgy.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gwbgfwxdt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtuksxehn.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/giaoizkat.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gwskarszu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/grajyuyft.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gtbhjjdvq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/ghfhcegla.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbroxzdfm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/giannuzup.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gqdxtzxdp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gguetsegz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gavtsxfql.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gadmmlens.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwtzmynbv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/ghsvmvfrp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gocwvomai.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwowajkjs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdzpnxgtv.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gbscxznxa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gaohhhcgf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfajkbbus.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gldtriuuc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gnvftwlmd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gpqsnshzj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/grtmljvbn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/glssgupze.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gujfawydx.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gvnagjzgi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gebjrihgi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/ggnshjllx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/grhgeognl.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gmahyazja.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gknapefdb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gmcvnmixr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/garisewfg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gkdtodroe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grcoufbtt.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gjoggmkwg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkkncyluj.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gpswvkcsw.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gafxspizt.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gcnnnzdbi.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/giegrlscw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gwpcasfcb.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/grhbaivwr.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gqwxnqibu.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/guossvdhm.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gasjnqwha.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/grjojdwzw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gqlkmqefa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gbdprnsot.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/geixvtigm.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gdrdqimnl.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gtmlytjgq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gsonrjtab.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gtapihhui.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/girnhzmnz.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gaxibdqwm.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gaplxrowx.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gcuugvilh.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gwgxkyxiz.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmidhmooq.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gnhfeuohu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/guajyvxyt.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gxtlpomhh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghxuqjuge.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gkbzfqsqy.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gjgvkwvox.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gidmnndku.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gsenqkmtn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzsnediji.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gorzdregp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsxmhoqlw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/ggqinlifj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gbgzogjka.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gmmghqakv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gmbhnmvji.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gyxwkyvgc.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjjitysah.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gbdkthxzw.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gljscypkc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gaiggvzpm.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gbpckvaaz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gfjfepgbi.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gcendfjsw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gngniicgp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpjggqavh.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gigrvjqfb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gxenghmxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/goiscxxji.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/glhvfarfp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gkjsjlblt.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gekjshbxf.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gsvjtcesp.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gzqyvmpqc.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gmtnqclmp.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gkxlztqsq.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gvqqqcuwl.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/goiofxkxa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/glbnmntre.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gfzueyvlz.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqivlcihz.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gxyidxsvw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/ghooiazve.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/glswzkwmf.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/ggxkousus.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gilebklzp.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gwqttgjmv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gbivzegvx.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gajpxoaid.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gdhdzwvje.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gfzhgcbiy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gbqklsmov.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gmdvjcwyl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gkvijdmam.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gcmxyhhoi.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/grhbzymrm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gclsxhbus.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/goczwuwyc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/grqymjnwl.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gnzvcqcer.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gxrbicnjx.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gdzcnixaf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gzxuozruz.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/goqemonxh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gztmizqaw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gmfhffate.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gmjxavrli.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gdwjmnpkg.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gaepzmkyr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gaturmcmh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxehlavpw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwyxcgfen.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/ghsbrzeuc.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxowrdrsi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gbinknexz.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gzzhqjhii.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gymecqpdm.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gmfhncvwb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzcubkxiu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gciwvhpvb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gumjzfsvb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjdcreesh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjivpvcut.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ggxebdsow.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gyfqpqbcp.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gkvolttbr.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gboweyzom.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gwinqbsci.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gchoqddoo.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwohilvgi.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ggyiyotrx.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gdxeaqsmd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gwwfwdxkk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gpcjdgsbo.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gkqddbgfh.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gtdfmixte.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gzvpxzoad.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/glhahhdxv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gfgivwhtq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gwjchdmdn.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gmjvsavei.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gezaojenz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gafdirpxt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gnelsjfns.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gervfjynp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gpgcowtcp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gvfgzkodg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gntklzjol.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gmwzwgaqo.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gczphwtaj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gzljkjvdd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gpsyjfdvn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/golqyrnnn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gnhoqjhiv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gssciophy.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/guwjuyvno.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/ggiyexuld.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/goawozcaa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/giygvcmho.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gtjpfbhjq.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gmrpfrfeu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gqbvemcwm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvtomtsib.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gewnwhbgf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvqtfxuza.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gtnmscfji.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/glvsqnhko.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gwzyfkmqw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gcmokknjf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gsydziimv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gwpumvqir.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/grxsmluob.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gepnjctzc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gbzkyfrbv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/ghmmvsnzo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gfefvqhfo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzpditokb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gnzrfdbzw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjbtsnpuj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtdbkjysb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/ginchmkes.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gmyhwpipl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gdcsfugej.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gvzrjxndi.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gytpsrzns.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gobdgfykz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gwcjyuwls.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gaftwzxyd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gawidiidc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gbhybjuuo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gvfzwqkwg.sHtML


<!-- 参考信息 -->