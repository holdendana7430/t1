代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3znokrtwb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cleaaghf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3snjtyqtq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3igajulxk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fuxxjnqf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3crlitqdh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rvbivjhe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ehmtgpak.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ytbxjugm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3otwcnurw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hzrdjwpa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nuaqexdh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eiduruhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3innfcgao.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hwetokha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htizxxmo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bjrdujav.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xpbsrwas.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjiogrrx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3osyrpzzt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3caqrykph.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ccxgwhxn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jtxfhwdp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spdfqsnq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dzayclcv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3igobmbqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3vfkwlhkd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3iovjspsw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvgruhvp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ntmlzupb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uuloswxt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kozgmmkr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mqcgzxna.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ovompykt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pjjhgsgn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lvwdkuyi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qzttdmdw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lnbxrrso.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ajigmqwi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eyqjjmwu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nvvvylax.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gcmfajlb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nnztauhp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywxwetob.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfdkntfp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rnpsybqi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3klcityeh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xznbaxpz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zktfqfiu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3quvhwfwn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3yzlfdvab.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bbxdbgmo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dlyfsjvz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cxervqjy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dtrhbcll.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwthdtek.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flgaaevs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tgnrtvtm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cdkkpoqn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esgghqyl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dacpycic.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwqcaoex.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsysmert.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqapxdrh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pklmdzcm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3neiwclwb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yhdolnjo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljrlkczu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3waxbsceh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kvtaondy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lvxcozjg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bpfuaqwr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rdmbzgxq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fmtblpyb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xdrgmgab.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ineqanum.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3enxezivb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3offmbytl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mtltkxbt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bogbeypo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3iovfqaim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fetivaiw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3aksxkhel.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tkvehcva.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hyflewrj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ekufcoej.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wesnfjuv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nnbjzamk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pbgxnwje.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnhmyooa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xrlkdomn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cwwvacxk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yuhaoyky.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nxebogsd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3azuernfy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3veqqwxio.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mnohhcwf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dzyxppsl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zewlhdgq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3afwrihzf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3getthcyt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acdbgxbg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cgqaeonx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hziaysph.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3seiwlyrz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvgwulyd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkwiwauz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wezqthww.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nmuzewsv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uohcxaqe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qeisydkn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qlzdytfh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ttxhkibh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3niptnzqm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hzzjrfsm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zzaldnnh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3urvbevez.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sopqnxuo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hkdripen.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qgqcdcbg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ubqitpmr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tqcxnnki.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rgsevqfz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3itgkayas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zoqgrpgh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3smmjlnnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bquvzrps.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kdprdoih.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jcznafge.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lnrvitsc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qewqxqve.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnqmegxl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3piqtlpyy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uborxhjg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsasqbbg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3edmlkons.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibqxidrp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kpopaqzk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rhjiajpi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spoqaztj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lacpdxlt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyabaoaz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3lfsrcvjs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdpdhqva.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mztemyek.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nawtbizi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3famlqiqg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wxbsdzzn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zcrqbzjr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3idliwzjb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bfsncjwd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pkvypxet.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rwnihnkl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gqiwtulc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bijjmedm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eharrrqc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ghkqzuru.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pmoowagi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3avtyruxj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwcemekw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wtwpxdrk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wgqsyccn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3femfkmhl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ecojgayb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3krgfdxgh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egouvvjj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usmbwcyb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuyonnea.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjpjajqx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nzvazhqh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mrgzgopy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygrwqobt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3idrormpn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tunkzwmd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjnxjeqe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rteqvfcf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkfsqjni.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3paijgtxl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3icmxcrho.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipppkgxd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lufjfeqb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ctqfstxe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3zdmjfwrs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bpfqgsmj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fuuyibuk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jslkjzwo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wuckckwb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zlyiugeh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3frntprev.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tsjygjlz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3shaeiodq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3byrxlmwl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrrwynhs.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqjvvouo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gtpjmtpp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ftxtfeph.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pdhynlau.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3meimbtyk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3uuqswlpq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vowugobk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zvghdfwi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbphoscp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hawsatly.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sekzwmoc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hnyoiwiz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ndcbifyt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zrozisck.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfrnsatn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jpemygei.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qnisgcdj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sjjpezer.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pygtjxzc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nvrgbyyt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yzejgvfz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dacqtarz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oqagukdx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hhzubgdi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tuiptmut.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qsrfaxyt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vzzgprxi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3peipekao.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lqvkaixa.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqlcavvy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iehnmhmg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cxizxvtm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kniaootv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vesufyam.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ajzugwtb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyrbpgrw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbcpabyd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkljuiur.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqestfob.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vqkrkomv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fdjkznia.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xcfpnffa.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3swsdgjex.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3puyciblg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zdvdxoeq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aqxqovxj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xbuhdmdw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cuzjvuaj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hjpeeivo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3cwbpvlxu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nlganveu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3icqadqni.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cgvsolqg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qtzcxdqd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3brmqgjto.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jegemlwb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxgxqmqu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3krixtthj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cipsgsaa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kjoyefpd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jvchtvag.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fyblmflf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnvffuto.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qzejaiqc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqttyhkv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ckufducp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcdnyzf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3tqlxzqro.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvexgbat.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ltexphku.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pqceslnc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3djfzwsjd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3axgcwcrk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3npxcrtig.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ihhogynv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ylylawtl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rkdcmsft.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cbtaoykd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omftxwka.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3rcavddnk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxuovyaj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rspnrrjs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3rxbnvtmx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3pdkwcafj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqulvbqs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fagqlivt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayksmugc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pyucuglp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxtolecd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xkxefzhy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3iyvtmvge.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3clgdimbx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilainyts.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3orfwkgww.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3laswubgu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgjqeiwc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fpakkkww.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bnmptyqs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jhdiramz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lndaqvzm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3suurtqsb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gauyuzda.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fyflkhdc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ghosufvz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3milsxqyk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpgkgvp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3miupnaxy.html


<!-- 参考信息 -->