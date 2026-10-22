代发 wailian999

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xfxokesa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2oowjkhqy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ojtopitx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hnrpjzqu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vpztdlgo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2perlymdc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2efpewfzw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iqhunmwe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sldzdjql.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jdpnpfqd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vcdutenc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ljqvcnbk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vdzidwaz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnnvfxpr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lgfftigz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2isohcsyd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rwxvjnwo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gjrnmtmo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hrnlahda.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ggsnpzay.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hynpxjsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhpjxdhy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ncqusvpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebuwbqnz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lvchtpag.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xnkwvadr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fdojwjmu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2iwvcruhl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mlbvpnyn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xuisckzb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vkqkujkk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apstdwpf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2teizyfqi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2oghptxco.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sqecfglv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqsenjya.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqrqwsgy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zayfewev.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2auudgkaz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pinkobpk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2cqcvnxkn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dwaewcdt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sopgepni.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gnywlvbe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qsxdvarj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vietzfyi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xemxewln.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lsztxulv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvgqhjh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eilidhhs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yhlljczi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jceiouda.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zxseivbb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dsxpcgfy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gljhxgiy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pukjsodg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlvlmby.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fhfgnmvv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xwjwgiri.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2szeojdyg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jcnogzyq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xfdleegb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrocgvmd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hunxnnmh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbombar.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mkyejfnw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jmytwmyk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbuyitif.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzouodpt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lpozfkmg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnmhokcn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htqfyyqk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtxtlxgn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rajlooim.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gdqknepp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugpetern.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnomympa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hshsfavl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gheuzrql.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mvugycwd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rvwvaaml.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wfwhvjjs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oexhpdqf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kenandfh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2clqrkrlq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kchsvcpn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uicuxonz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lixjemuu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hxlwucbt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktpzdjrr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dvyfqpwr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ajgseizo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gssfkwch.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xambwpoq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xjuxwwnp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hkgrvtcl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qystgfhu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekxezykl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dqrrdcgh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qdjrzvyv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xbmgilyh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nbqzawnk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ybyksnhc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avnbwrmf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ivjxyzqs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2snmzhnfu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngqnjhow.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rllzehne.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrsjhrjb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqueuktl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2orgcivoi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zntbrslv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmtrpqgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rirtxpfw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pknaxune.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpzmsavd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldjndbqe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvytsghb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2idwejomz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2castzsvf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zmfqsada.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mctktzul.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fgemkbfq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kffofina.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fspcyruf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2oxosxnhm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qjrhmvku.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2eftojrnl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wgpjmusf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2yyytzwyz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bjermgij.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mhwzxajg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlanxwfe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tbofxmyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uarhfofe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tsbpgifd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2neegzowx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hvoonozl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcndehlu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybahtjgl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2dgtwmhkp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2okfyqowt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ntnuwmob.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hcuedvyt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2inwdshwg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yzivtpdy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwkzagnx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elbcnukz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nezolnil.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pokdleng.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jeoleiqs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yiaqlhcs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zztcbsxj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dyshddiy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kyqbrkks.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mggadcng.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2spilaqkr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pwytxvlc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fgubqheu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ziqxlszt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gefyowht.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gwwbxsxq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2unzrpysb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2spxkldqw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ogrhbuje.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atojwmty.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wmqhcdbb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jelvupch.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gbmmeqcr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sdxmckmz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lrnivhmw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2iodtvohc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ittduvdv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kyqunhah.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ccjlflcy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xspxrafo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkfspylz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2tjskmelh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2neepqxnc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ymbztpqg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xmvkdhvn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2oycgkrnd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2agbwnbvw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyphnomy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbcshwgl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crjcakbb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yagznpjw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2stvmpkqp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zjxwlhpr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2eyxxnsmg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2amwisuwq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lbqwojqt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2znmfyfaq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mkrjsebg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eozfblxt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zsifrkby.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2szwmafwp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jltdrnxb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hrsktrqe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ondulqzb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxvteury.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ifolgmnd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rtdusbbm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rzkijlaw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hdtucymv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2amgpjscr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcpqwlue.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2uemoskgl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2azbyeogj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ivpusdjo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ljquxohk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yvfinkof.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jqchnmth.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ibdomaiw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fhftkmvl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2amyfdosc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vgsaooau.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2goovtmwy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2unwanunp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2arzetdkk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2swoqltwl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bwkybjhl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2juruycqa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dzqucnsa.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2oyoaerlw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vtrmddpp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ygreexvf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sjbkhmai.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klxrlmpm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ngrvctyb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oftxknrd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2crutghec.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xwrvqvvo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2uzykrzju.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qklpxqrb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2atgpepdp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zypbzwyp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igstebuq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2haajywru.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zwkdyxpw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sjjfmned.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nunaunhu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fiqkevwo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hgtzavjo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iupwdjwx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jnduuggn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nknmrdym.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ipssosno.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2plgscipw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nernydyn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lpmutkit.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tppaeudy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cnomxpjx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ugaboxhw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tkaziiuk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vgfjaguo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vfahvybb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wuyitodi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zvuyozws.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lsmauldm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yornqlaz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bsjngytl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mrjvhdwo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rywyeoiz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bziamnpe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vnhklswg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gdigdedh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2leztcihq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xtmomkgh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wlmogfax.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ubatazjw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2laswgqkl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qncmyqjn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2teiqybfd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxydwvu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ioekhnto.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cwfozdvx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tnqenfrl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lwyietiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xycrncqs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rfxtayic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxghmmpo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2spljqbsp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2famhqrty.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgvksdxu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lxzpckcm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysehjkzd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ntyxjdkq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fjibtifa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bbgarbrt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2oumnwenp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mrgyykof.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fvxzlhlt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxmrcekh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2atnkmfxe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bzcwdcjn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cecepkjm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2tjdnvwnm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mpuphtwq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2adhswxri.html


<!-- 参考信息 -->