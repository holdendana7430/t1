代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jssiirxu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3noebipxe.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tizvmlso.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3celmjbpf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3usoaozbg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zujbijhq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3skzactmq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rreecusr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gwduykin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wwyejhds.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wneqzxjf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fapsqrtn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wroyhgdx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3twanjoho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kscsnklu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fnxxsgpv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yhmpypdc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bkgmgluo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qsdqtivn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rsxmrbbr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tiupebpc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3psdiozzt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mkkfpbuv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vwmvygbo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dpgwxwvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adcsyqzu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ajtowlad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgaynbkq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3njmyyquk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cohuqhti.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zkhvdgec.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mxkioerm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vlmgqapy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vnwvrmll.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ycriwteg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcumkszx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygeblrqf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aijrmfio.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3czhlkiti.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zlkrhqqc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybyinjpj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vagjlxvq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wbppyhja.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kscufymq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sbpxjfjh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fwrzymqn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gbxqlrak.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hkwaaubi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nbsedpda.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gjabtykw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jpzttmac.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vijjtxqi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fmtiqbbm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3illhohig.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jclkgdzw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zoqhhccz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fmayspjp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3phivjzrz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dawlvvtt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wdqtjbpf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lerrboiy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fmtlmynr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uqvnjczb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pqmjzsgs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lcddwgat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lxhwwbev.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygpmhaks.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3huciakna.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhychfmp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yguzxgfz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3usnozetz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbzhrosa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuiihome.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ntchdtgt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btbgomzf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sakglzge.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rujpgysv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtflalmg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ltbnjywy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjjzbxkv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxajkcac.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ughaubfu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fvnmcipg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3crhapvqc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dseqnweh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kloxbmxu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3peuanawk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vuyzpbny.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ycnsjjkm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dknqtiom.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ykfwdbzh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3slyjeoou.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ftaahbmh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rqjrogbt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ktkbcxho.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sezirahv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qpedphmm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3meqglktj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3osjlvtbz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3iohojlvp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3egnbwjrv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prkbwyki.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ivrlwkei.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hfobyqje.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3exvvkasi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbwkjizx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ojanorri.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tosvkugt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zotxrwnv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3olrirjdc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxmudgbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbikjgiu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqrknmpt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndjpmmcs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mhagzhtw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdjhaxoi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihsqfdqr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yycdimdm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tbwwpfml.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3chxrsvzt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iwrglhkh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wyzbgtqo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fteavloy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3udsjddpn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xxtjgqxh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbqnsxuk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fdnklhmw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iyqjpdrh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wuckmqbj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lumheaco.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zyrqbqhp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3satyinqv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dyyflcgn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxjlea.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dysywhtq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qsopmwff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afpvozty.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cbrwprdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtxvdoxm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ruqozatb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dxlcaxzm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgbmazrh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3marqsehe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnueqpqv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3phgpmfqo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ldpjwdhe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mxmwcqpn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecqkfwue.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yknvptms.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zvmzjhxx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yflwistn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3alqxppwn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvtkqyom.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gvdarqiy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kdvfnfbf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qorqwbgi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhjpxpt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3txphzbmy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hvufwmju.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kkyczyxg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3djxshqgy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3frfwqsqz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hmvgvayl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xydibtwb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qwcgcocn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vcsqcdvo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yvwdjonf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wjghfuja.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hwsblwci.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lzqmkaub.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hyauinpj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grmipkzr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jlrhuvej.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zcznmeib.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nkoqzwtl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iyvsujxc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vuyeahkz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rnwftojo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3twugatno.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fyeerlxy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xxrznuoe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bnknbqrg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bhjlfcnp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqwvggdj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ejdbezhh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xzyphpri.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3emctcmci.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uibsoiwj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqhcdxfx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmeduqsd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3njtsjcux.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zhjmipyz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fgvmuhtp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fuofwytx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3msgugvcn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wwqtrcvr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nmvhojyk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nvvftumh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rqxyykzc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3scilrohf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3umlymkih.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bcaegayd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qxmnpzph.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3sdykvdnb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwkqggcj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeheyoaf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jkzscsuy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydeshcjp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qpxvbupd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mgrawrov.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fvxvical.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3iezggobt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rhpslkyp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kuwzyefr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vcdxbilg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gzhvrqkw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kwcyeqmm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jozzydyj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gqkekejb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3osdlhwlt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3haxvazgr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ajjsczjq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eqhdftwl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nmfzwwvg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3adhflrov.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mvdzxinh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dyuhjnfc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3djttvgwv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hnewqxby.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3udjkhucl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3bnmqocdb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klblhpmr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uukjkcii.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mgoldtxv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oukldfax.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cxyayvlg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3sgnncedy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rcjojypg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wwhamozs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ohfydscq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghmggsxl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xwkcakjt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmubffch.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3evbajaie.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ifhhbtiz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qcknjvng.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sbxlddop.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3eqquvfrd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nuptscrl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gjuqrdiv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cfohjijg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3reoclsup.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lhknairg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dnhgnzkt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rksgpxhx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dgadddgu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gvxsawwd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3crnbelmr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3erbrjmuo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pdduubry.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kvndcgrd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmaroawi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dkggwynm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rckbffvn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3brknbafu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3crlqmupx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fjdiswjr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzqkbcle.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dmpksrkt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjfbstp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3sfqmkwhi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jrskaunh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nwpurumg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3evfbaday.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3phjadada.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3boufnpyf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3orqbnjym.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bgpjfeuq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vhjmbwcw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fynslzvh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vfudmdax.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3trovltzl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bsraypbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtiuljhm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rftwiowd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttqbumgi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3autwwnxi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tuyijyow.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsnczjzk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3idiklggo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3axqcujsy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ypdummis.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3farzurau.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3dohgudjo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvmexrkb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xfmtzcpv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3glwttmqx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtxvxmot.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czcyqlji.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lojognfm.html


<!-- 参考信息 -->