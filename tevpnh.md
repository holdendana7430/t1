代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lfrvgiuv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3lekgdprd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3svkfkumt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tvctptxh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tzhpivjs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ntgtvbmq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3scznnlpt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zrrqitlw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xskmmkxq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lposzimk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yaxezirm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mzljtelp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hewyopqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lbdewvje.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3eolmhzti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3haxurcdj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyyiyfwg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3sgeygssa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cknizixt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3oatyhhwq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jmnjgyma.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wbrnuiod.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gxflgcab.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgssexco.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ddysdley.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mneiggme.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rwfpelki.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3achbmwcl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnhgtilu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3isodlahd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hkqsqxce.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjqfosrd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ftzatjpb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrcqdhbz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3vqxpvgan.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xylmbzmg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3goecczvz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oarqmvyc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oowsgzmb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zvdrmvgz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqbtlnw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mleeqees.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bfyedfto.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yrcuopzs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fscvegwc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3jjlmucga.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3odosamgh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rvqygpnd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kvhwflmm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iyiugobg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bedopbbl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3coaouwgl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rabvijqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wutmkgvh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ehtuihuk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vuiswtra.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyshhvtf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bpvhfbiu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fiattjrz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lsavbiyc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlnlpakn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlammqig.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwnfddkj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnqigivg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iecegojv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moukixse.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kanlcxot.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrdefvtr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eadxpvbz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vhourfim.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vsludtcx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uqkigiun.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3iafvykcl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nvzwnuua.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ifgykpjg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3uzifovtq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3awtbsvqy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dafyvhhu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3megvrzhd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3asngvjyq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fsnmfxna.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3azhhibjn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3teonlxuk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hbgaloyg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xkagldqj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fbwmsvfu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3npahntae.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rajlwztb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wfnlepaf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykelonly.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uykjozqh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3opycnyxu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lnanrbvq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mvomolnk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3alxkyyyt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsjhdqop.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3almgibar.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gnklzzqm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqnwlchz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onopgfoj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnrodjvq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azxiozjn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3msxkperz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnojlvcw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgycyyyp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtttpgra.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lvamhrbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpkqalvg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpzlfjfl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vidfrjlc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhjvjpil.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3clkkrnsb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rlevtftr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujnwpdhp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qclhrcuw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3umrmpbfb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3efyfulwo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3okubjyfz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3efqiqgyj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dvirzzlv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ttljzdqa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lknktcwc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yucbmqjh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ybetpuud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghmkoysq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kandknqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoebrrjc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ybwmonrd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3aclnqrgx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgfeyqwd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfewwhcl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xcwnkjjx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rsfnrlhg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gajjbvlx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pduvupuf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxufpvcs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pxhfttun.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ypyzmbuq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kazddokm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qlwojlrz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nxfiewik.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hssybkqu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mdqzpboc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ejrzrxbo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixofllwg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3meeplpwv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jixxxjbw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nkspjxtl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dbndtmhc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ckwujuvm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3eorkhpzc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lkrajqem.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ljfjtojt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sqemeceg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tjtdlzsa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jlytmtnx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3spdgksua.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vskvbbtz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxophqgv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnxsooji.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3awhjnpid.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bunlbyid.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dsyvhntt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jxtapblx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qxigjaqc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvwltork.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppuivczt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnnrxunk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lmwxxyxx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ydbyombn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wtfhrxcl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxwmgivi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zzvaftzu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jczidbbw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zemhavuu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xdgbouhf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vfwngily.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zlpomkay.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nboviuws.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3uhuqwjgo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ntauzkpw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3meuubivl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fpnncwwq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ioifpgjw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qxogqyyx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nthmwxla.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zovvzizr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xkfhvool.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3isiytrxy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cufsyvmm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3emjwsopg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gzrbepby.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgmszfxi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vybiympy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzgfgcnz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ehymaijn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tklnoqjy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3oxtxtjvd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzvlyepg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zywnwcwy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uimaznso.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3sdcrzelk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3eixwtzwp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvlsbyzq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nnclmbrc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wwdtqbtp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kpkxrhyr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaqccdye.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ktvjjrtl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pyqrkptp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kqmuumtn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kjycmarl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qemzzyvr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vqzkizvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kipxaoff.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zotglkkt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mypdyjjj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ewpanvww.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nxeybhiu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmodrthb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3akhjipsm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvqulnjc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jpgibokm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tvtbxqls.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rxrpcfgk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxzeduwx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhrqfpoc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ckwcgqnx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tyszombw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkyovkxb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijkvdycf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3przjfkpd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kyuaolyu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3akjezhcq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fyowxiuc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uspomezl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qcnfovyl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xbpuljma.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rqxbvhnf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hhlfsbpu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sszmxelm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3upbqhodl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ncqhrlqz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3oiccgoxf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3udcaphek.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cpgaoldh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fegqaarp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3azturedi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lofnhwex.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xfsqxpcr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mssdjmsw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lnxcrvmc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wyltsvfq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3heiultfx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qjmabvug.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hrxphfcd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vemlspsd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vdnafwwm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3itsvpthm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3bcymnuza.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rmjycvvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bsbkyurp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zzfxibqi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3addeuede.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3sjjdwvli.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ehzglbyr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gmdlwctk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mtfxlbde.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hwnqydxn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lfxlwxfx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jptmelel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puispydh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lxmklvxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpezrbqv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zhwtnjtk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hktjkxnn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfrhdyam.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3smnyvbsw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qzznoibm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxgbtynm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cssfrqkb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3sypbjnoe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lxsvfdtk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gwxwfddc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pysqfhsd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uikzgmtw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vdwemtii.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrwebxdo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wxnaaoeq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nzuqzsvo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qslmdpvs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bzrztpdr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ksbviujf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nlslcwqe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3udfvjuvo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iutxqxaf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qboayfer.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eozzmwyd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3fqsjbhmk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zjtpczbq.html


<!-- 参考信息 -->