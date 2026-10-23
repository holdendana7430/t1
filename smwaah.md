代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbvdzyei.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ccjukenc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3izivwxnv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hukfhwyj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yfgvpucz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tllycidj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aaulxmos.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3soirfdtv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3agmnphcj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jauhrhsi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wjdpfgrp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3arsggscr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3eoeauayx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vhgrpsmj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qneptfup.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rnhaokei.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jxybmdai.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hekmmsiu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3iuywnbmw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rotidgii.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qqssjovu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmeygpzw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jefhzovj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brinuime.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wugcxebj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3bkohrnno.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mpbixete.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qgmizmga.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hoqcoirz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3krsnvntf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xjzkhkdv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3murnwzms.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zquomkmm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vxasasab.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ycqowznd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nueqluuv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nclgiaou.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dnydjktt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qlszyhcf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3btiocqdc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wvgorvsz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cpzkxleo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ofbgkphz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hdjidope.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qqmtzokz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xezksvjf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mbilnqcg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3mfxvabwn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3niqvhjsi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3aripfeuh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3avremqqy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3tztxnbai.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqdxnu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wnkpbhio.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xauincsx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oucwjxvj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ngahtunv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fbfqojqo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gynjmizc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vgpizeqr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qarpexrx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wlcwirta.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3netovvcj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3grcxvrxe.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxytaxpp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ympzfvoz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rgifigjk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqfxasbk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3riwgtxvc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zuwsabpy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukodvssy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qelftbrr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhrzeihq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmzephpj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3euevwbfx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzmnqpjx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ospwajuz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3chjgrdkr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pviocvya.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cmsxqrwt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bonhnseb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3egympkvj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dbpryasg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dmctycax.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wbjseixd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3usnghsqm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3agyivmkm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cgyueghf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wwomlthq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqojhguy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3epebhxya.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qvmrpcyn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iubzkdqf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aovnbnti.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3lltdvwzq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3exsgtlzd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qldvsfnm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmifhjyy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nppiaccp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vqqookhe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tsnxluqi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kcxcnqmz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3abmpbomm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awuctdui.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ndiboapv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3soslkibz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mpfrxkbi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3veadfedy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pirpixbb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlymlhlq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jcaifaoj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uverksrb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqawxhyh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhexwspp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmrbwxlj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlsiohui.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qdcbnyqa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lguhtfwr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgjqiyxh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3buxhonps.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kbshexri.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwkcjtve.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ezonzcyv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3modduoew.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3okuvqxsv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3nuggkdmz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mkggwson.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rzcnpezk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hjordolu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3uusxwnak.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3iujlajhx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mufujcky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsemkurd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ninuucdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylrielyy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vxjkqpbk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qltvwbak.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpatlzjz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srtmijmd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dnebqicg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ungiqslc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jfnynwvy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fhidkneg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tflevvkq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxtvaufd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gksrjtmg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jqqfhwaz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3auwkmwmv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeqxpvtj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3saxzeikh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mmdwlgwe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovrvibsj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dulacrsi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mdmqssdx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lfdtivkp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bnsnyuno.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3whillpsv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yzeymjbu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ghbqqezu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ihdhtzbm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hqwxwoep.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3valjmipu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lxmeaoxy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zklkypkb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xstyzjse.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hqrlpeeh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wrgmvwac.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dzkfksfg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bvhosnau.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdfjpyue.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mhydjgpq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3urnszved.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rtdmfoyu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3muihsapa.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuijsvfj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yelbxbbs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ogkhnkty.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ntkzsxpk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ozmoiggg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jluwmsma.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nzlmziyr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ibekynhx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fwxjkxiu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xrerowam.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtpfxfv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yimvrqoc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pjbdsrde.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wvrsnozf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qhnyzptf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3anejyonf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lnuzrbyw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3sbylrull.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vnretsop.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ouylvktt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pzceerup.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rvovewrc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qvulvpru.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kysntgcb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jqsjfxog.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tzyivwig.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqktuwqy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zchcdrwx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxqqtnbp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dtlmvjug.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wbodwlgp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfbknhnb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cshjidqj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gphghzsg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3blgovdkr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zfsunukw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qxlpamca.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fijwfabk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pdjkjuei.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jnfqbwsu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jpddmavg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ailzypji.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wndfujpi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vgnjmaua.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ewnfznmd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zrfufyta.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nofoplir.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ycipnryq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cwvafkjw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fzablsim.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dxsxgslg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zujsdnvy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lqkhigue.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wessincj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yagjvusp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3luaqnchp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjlqhprm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ogrmackw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gtgtnwnm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsiemfvf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aowgqatc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tytvixdg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bpkkbxji.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htbyauin.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmakmoft.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3scbqdwnz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fpswosea.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbnkqcte.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rknvdvqy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jjacharj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zdylbdkb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndtqsmwq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gagqaqja.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3regoigte.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3osdvgdkf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vgwujhte.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wdgkeyic.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uljkomxy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qbdeaczi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3teljdqfq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nzwgijhl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ccuudzkf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pgcyaxqu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kymiwhed.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3binkwvto.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lpyafrwk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3owjcfbhm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3giuhxufc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wydxhfbb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3eugiqvor.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lonjfxxs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wegxcjjl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ovxbfetn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vuojvbkt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3tgevczdk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3edivvxgp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ubfcmpek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nwipugvr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qssuzorq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3iacdpjxu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lxdnikds.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xjabpccf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3iolaxniz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3flcoocwh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kdbnwxbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcflyrcp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3buyhzvgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcadfnul.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3stgozcyr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sfdrssix.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzqjggzs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvnypuuz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zolcdvdi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vtogqfmq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3sujzruwl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3tbfmezud.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jaxdshmy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3egnysnvd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kzhajnqh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hqbcvnlu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdkwnzyf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgwzwble.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ccgwlcib.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3skwwaxiw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jlnknmwc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hjdjsiuv.html


<!-- 参考信息 -->