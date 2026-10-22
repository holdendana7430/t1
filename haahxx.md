代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaakwyof.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yuwmeios.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lejgwcag.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kdtuggyb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ewrpkmiz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zdadjvyo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wcnrdmth.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nloyrpkj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xnmgpowb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rsxnlhje.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jjgmjsim.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2imulccwh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wtbpssro.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqgoqhsl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qfruyhji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vqzfymhx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lvhvknxq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bwmsbkkd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wifiyepc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ovpimjuo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2afbvmalx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plifkdjr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hsgahucn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exrvfjnq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hsxzgypm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qylzgwla.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vrvyxjpi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2waabtgpk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2okjyoplu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtpfpfbq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qjikzwtn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gridjbre.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yuwpkcgl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qowxpxad.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mvsxrjlw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2stmvcxav.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2teumlsen.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kjqoqgrw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fjmjzcqs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dwhfhxhb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lndysapa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2txxfoyud.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2onizcugo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dltulayr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kawmkalt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hwuaqcwk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sxqewpea.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vazybbzt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cmthjxds.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jysjyqex.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uyiewqvn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2trhpdnlk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cpwbbkbl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2znlawmbz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gjlghsey.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dfvkcejq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgaaaqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gdaabiev.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2favqrbod.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2utsgfrrz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2icbnubbn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jdrokafz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2orsdywrt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtsqqrcm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyhjbevr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xygqpgzi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ljokomih.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jswjuuzu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yyssougf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlikizqu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icbapetg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhgviqws.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gaiduiig.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elvsgptu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tllyvwqt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fekztytp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbdpjcny.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxknvmdd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ccywiuhu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2amltdkua.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2auadgqzm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ydsxfctt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yciigtnl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2sewhjort.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ohngkezd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qssxthbs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2eiofyrsm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dzrgbtwy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2musjvtwj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2csvsslro.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvphyduy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xmqlcfwv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sgzictmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pesfnwbg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kbkrxhkh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ynoueafy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2idofsotx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckmrzton.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlqikdok.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lnovjvsw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mwknmcob.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gdueidfy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zxckjfmm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifpmrihc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gqpswzrk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fikrgwnn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijbobakf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jyidtmqb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzamxpak.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jmpyzwmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kcwswejf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eymmgjak.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2beflnzaj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hslnmbpt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqghzrza.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwziaasi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2blczucyh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vltbhdql.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2grkfbgna.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rgyzmycc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fmgibzqz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtdohthu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fzftmedd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mkksxatv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gfnnldpm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ufhqzqji.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cclchlhc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2djsjaalk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mqfiqzow.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bthqrueb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wtzazrja.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hixcxfww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uiciettn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lhuyrvki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifqqogrz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gqsxtzhh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dlcwobmd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2liugwqng.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2szunkktj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hutkxkkp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wikqlnpd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2phcipzrr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eecxgmiq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zatqymlr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nadtummz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zymuakha.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pgkymnxe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eytycdcm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzkxelth.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulwdwari.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wcmhmoxs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yjleblwi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avwztlix.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rktghlgf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vsquyxzh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xfftecnz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ezegnkev.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mjzalees.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tbzmrsjm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wszbehxg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lrnwkulq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wnojfsyu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2krwiyfpp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zsgvxteg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bchbxjml.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcpldiiq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yujvlwuc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgkqmbxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2msxtfcgw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmrhzfno.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2spxszple.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hvgngims.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vrvofcwh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2avnarddo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdmkxpqg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jfeescfn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2siyejkvw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2sicjzfrh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2unxlpdnv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlulxmrg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2azhmpeey.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2udugrxka.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2svyfzrte.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlnirimk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2goyrowmi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgsovefy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2buxoqjek.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qstmjefr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vrppmeqa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2calxqxdk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2isejnsld.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xjisfaam.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ojrophud.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tupolyht.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gqvjvnax.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sfzozxcx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2oqybzdnu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lwllfcpa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cayjenam.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yzeuyukx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkiacwxg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbdycypn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2aptidcju.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuwkjxpj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jfqryjsq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ebwncnxa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jqvdpnxv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cmpsszhy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cmuoflzj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2shamhkrr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iqowrmjh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfhmfpya.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcodlfau.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hmofsuno.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtpgdarm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vkawjdtn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wqjdvjpt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2bchhbnmb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eaghhsdo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kxbajxvm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2snilpogd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2txnavain.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wxukakcu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ntgjytor.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2uqufrmsh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2aokfwgho.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dbkjmeht.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2csndggva.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dgijilry.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnrbvmos.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2owvttjns.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yssqnfvc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ktvyrvzb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fgdzcaxa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ccifogwh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tlnrhvha.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gddozaxd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueotbzmz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnvvxznm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxqdtnfm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ahqobkaj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgakyimb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ljmegryh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ojtjdbzh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pttdbhav.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sowzkdxx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2betjkkrf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2axymyjos.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rlogwjjx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hciwmarr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2elsrjovj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2oufeebzo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yhwoesmr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vhfuupsb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lsmwwgow.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2edbdzhgw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ewmzmsgt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2eewlithn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vimgqjwj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ldmhviob.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lntkowdx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jobcxiek.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wydwjoxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2arnfixiz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rwmxjbng.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ecjqpmjy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fulxwklp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2onmzzuni.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sbsjfpup.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kixglsxx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2omrkrczg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2uemtxszr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2efkkwgfq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2itznbzxt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ibcgqbuj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qwrmiupw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jvagaaja.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rgzzdbax.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uenwqtrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aotamxnn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2upqvinao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfxkkkrl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2viydghql.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jvlvhpeq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qqquionf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlryhwch.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2blatjccx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvpuckjf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fuurpoll.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2heqpyvso.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2crtyxeuw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fygmmbyr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2heegfdyk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wmxycttg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eaelyile.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tautfmug.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2okzgcerl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dizvblqd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2indhzfrr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2buzxwzyc.html


<!-- 参考信息 -->