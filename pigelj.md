代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tveobnze.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yuduojyr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rudelrsd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ydukkapb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zlqhhvia.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hgqrbtpm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wentiqmc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rumxlhnm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3fofrlbni.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3oozykpfv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3banibbkm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iizwyxhq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3raiuicfq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zrrfwhyu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uqfmjrmn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3eulgljwo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3twvonpcd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tzwaikdf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mjutvqaw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3himyyabg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jtkpaewf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3asgruszl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gpfauzmg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xagzsywe.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jwpqzjdu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wtqjoens.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3opwnlzcq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3frxhshhc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bqrpnviz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wgigtupk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lhjbxcvl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uepugbyj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ixeswrnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvvetill.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3daqzlach.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjvphsrm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mnqdxini.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3yheucpzb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ydwzlbgs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pxseibbi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yxanhlds.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nfwibltn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tpwbokkc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3arwanfui.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kzcrcran.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywgxagtf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3sxjatjgm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vcxawyxb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bgzdejqr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gsfgqkxe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hezhryoq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gdtgcdyw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kfdalaaf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nlxoxwng.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ddukbntq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wljxxawg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yasqsdwr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jmyciunl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3looykahz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bizddewy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmwxidf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kpjnhuxt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dtzfsgyn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmmnkzmn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3genkurgc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3oknprpla.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cdxdufue.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tuzbrcat.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lvrnqxxb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bveulfou.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zwbkkgnp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vszkgegj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vxewktxc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zwdjtzes.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gwrmmlwn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vywsghda.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhggwlfk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jaimciqj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qlvjfkma.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fazjnsfe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oojwjnrn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ieynlfcb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkzpiwue.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fevcoyqt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkamdxvy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mlyjdqrv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3igeyiqhg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trtfkutz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmqadwzf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bbikynqc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dybijvsl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mrojlxkn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uajacyjq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hlmtifjl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pcxcktcv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3spjopnbp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3waijwbon.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3snkldmsx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tytfamkk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3adfpkwkv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtkckzl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gortidvg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yaagyswx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rdlanccx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oaljbdts.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zkyepbnh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fmetlxar.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dszuriee.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fwmvaunh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zduodnyq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ldzvpgnq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ngylznai.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3aiiwjjnw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwgikrjp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wiaohblh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mchiigcu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kgsigqlr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zqxskyhg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivoiwshw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3txhbiyfw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbhxekyh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbsohozz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rhotbjke.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzbwctmg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oocjzerp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwnwceqg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qhqqdcbc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufcukqxp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pqbncoob.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eypwmbay.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzezueko.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zjnlggwe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ufumpfkx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnxqocil.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3yygsxwaj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kzgwdjcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rzorzxuh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wiwemsfm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gafocqnr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bkgghlvm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3fmthvrpy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zmhldawm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vbnjcxut.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pzucurrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhoiuagf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xysgjgor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhqdbpks.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wjzbonkx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hohpemaf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3oklbqqok.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvekpfwq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ydjckcvs.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvkmfksx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zzxsqwsz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rnuuxiwd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wvilueiq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ueizjsxs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ajxgoufe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grynmwml.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jabdsxpv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3exrnmldv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3veqkscsi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gnhmbprf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dcdezkjt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3deqknwxx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fdcpprmj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wpnuonos.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zwltcxyc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ynpjqipi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fbhbqocv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gilarezr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jdwskved.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ymhxmbhp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kadjuhze.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3scfxprfh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cepcuxff.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mqkrgely.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bmpuvbcn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hprbcnac.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tomhgyuo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dxntgcfs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gymmmeeb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pdgnegue.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wctsvitm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pmcrchfz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sutcrafz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptzftbor.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sredoneo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kesnteic.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xcbvczdn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xevxdhjc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwfydxdq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zkmevhjo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ochdnguy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuqadgzc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsadxzbj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fsmjrbcy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nstrqqev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mhishelm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hpduqxob.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iwjmxhjf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qeljtywl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sqtupght.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ahpzbxwb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xvunwkry.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vtjxuzcd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gqmlskee.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ahftzzxk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uiovqewo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ioikmmvp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ooywffuo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zvnjplpn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3srbntxdt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jldsuqjo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lkuswfle.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksxqrutk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ltabcofg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lbwzturv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hknxebyb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3aelrmbxo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qrosuscu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jdigumug.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3osmvvkie.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyelxjnn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujljdqqi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3oeocyabg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ymrqbuzl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzvvuzsx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qmivxyay.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nkkwrngh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vnwnbbvq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mcgzyxdo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3brbovqqi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rvzbebcj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3henpthqc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uxhopgws.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zgwyfnjh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3shwfivnb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3stbpnbbp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unqvktct.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aieihlmm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uugvnxli.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vahjxjor.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fxtlqgdb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3undfgely.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fulzqcea.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ikxkzelb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3horwlzxq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ntkypclw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yvxbndtl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdfdrcdn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ayglasob.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wkgvedaj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqoyvkfa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dxbobrdn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rtqfzrjv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pzrbwnto.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qgkzdvvp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ggpihhch.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kjnylnek.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aryxxvqq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3frctajyd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fazfcyvy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3aziibgnw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xyjdzfhb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3acuwnauw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3swojarno.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3oxmtswnn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3riiblrwn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxlqqvii.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjflzgt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vznleqvy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3aqwazpgz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rwrxcmyz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xtqepmni.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csqkptfg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hllwrnzf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hkflllis.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qqiavtzm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3frwbgvsk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wxzaeqtp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zhytoquq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ftomrfrt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3hfvolajf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3whgdxtkz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ugfoghfy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dybkoysg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vnebzqup.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tcyurirk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hkmwrdkk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3znpwikng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egvpantc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uzrvhthr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujotiovu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jamknozj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xkhitsya.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjjevqkc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wiyvwsop.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sorvhrfj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3stgpfhtj.html


<!-- 参考信息 -->