代发 wailian999

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3vlwbxjqk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mgfhdfyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lwztrkap.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3avpqwnjr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wlccjere.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dshwbasn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ebdtzmww.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ybzcyhoe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fjhbaqom.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ezueimez.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xsifwsnz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bpchodtx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mprpsdtk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvmpmdai.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nujaniqz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yhzdgtdq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eddetzuz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vhmbcrov.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qinbpkkk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3saejrrae.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qqttvicd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmqcdmwm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zioxcwcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icposume.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kyzwonlt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fhkxrbyj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yhrdggwy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3widdvhlm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gevvlxxu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xrxuoxwy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3skzfkazb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxjaowqo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bmrgoqor.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3koljxdnt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zaracxgb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzjdvglm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbjujwkk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isbzawze.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3btdfywil.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gcmewpec.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mqzldjij.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ljirikto.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kznstyhv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fcymnune.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wngtutel.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hpevegip.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rpyyifqq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lplaiyja.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3uftvsngc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dpvxcfai.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pllpjfig.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tflyuins.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kmuvbtzk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cxeqicke.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zgreywfm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3micbhjmo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3udkyhwhu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3egapndif.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cmpflvpj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vjajgymn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pdvdqskx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rlnqtbsv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kvjzhpsr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdalciqq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nowwcnwu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wxcrepml.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dxpwqcje.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3girryzpc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3keqcqntc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrfgdvsz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isqpyzpu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsaatgge.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jivjigtr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jldsbpge.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jkahlqsf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwvjbmzi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3reeizltf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tixcwxgd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xhdplngh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ehniterm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hrowubta.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ekascznl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ioggbodv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hopuabjf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hxjgtcra.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ngrskwgr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3neodoxjv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ivjtopir.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3aiiaqhdl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihjyqmnj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3invofnwd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hbyqbdea.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kosdrnkf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3adywfutb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yikcqgme.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3iujcsokl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3difrzjuj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffrlvjhk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wsqhdjfi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rcyesvjy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hwjzrhel.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aajqektl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wskycyvc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkcicrsi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xlinlnrh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zflbnfdj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxapggle.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nanfcdpq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrimhywq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azabvbks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aksfhatv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xewuskrw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrgnsljc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmcmtavp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pkbdahmb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuedhplj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qvzcuucw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztmteoyl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjnghrcu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cdqgwgkp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ibxvfevq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrbbcqkd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3pqktwaxf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wlwfalvw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3cmgyvjpn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qureolfe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fwsxfcgt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dqdkrajo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3oqtfzrrk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3evgetsch.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3czvrkvie.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3uvphggof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpkxqems.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uvumqryj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ueuecxlt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dxnrzegd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3udexyioz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wasivgeg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fslnhuqn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kxqdqdsy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3grmcpbkk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uzkghyjq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3oqjrmsns.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lfwxpand.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3phlxmwtg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xbkdbsnt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkjduwfq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hkkdlwor.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffsjksen.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooxzvcda.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gctcbchb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ayenxvaz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzcvmxbf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hfecyinj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nvorrxng.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tccankgy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3itkfbssa.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3oszmhzdw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xykugays.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3oergjatt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ftffzppc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qbwauaop.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tsopdmzp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bkpohqju.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ulerwatk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kkmwkehy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pexvkykd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bodcxpvf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wxtggtlg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3miewwzyh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dkrhadiw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3khkggowo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wxppwnoc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3npnkkixq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3upspwnle.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rzbxcxnc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wqopahly.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3smuqfice.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tywigyco.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vhvocewm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dwexoxvv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pscabnpp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jnogbszi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzkimtzc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwlbnjdu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dogtosxh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qrzepydf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3stzlaitl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3asfrmamm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cdvkzqdr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zjiydrrs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3medfopfm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mpownvnk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3shjfrgxq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xdnrhxhm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wehxtmgt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zzbjzhct.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xmvwvmmp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ikxcyjhc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kjpnpkfg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mwqwysgi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rmvnbntk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3pywfceal.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gnadvrhu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ddcyvhcv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mypvuafu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkwulsss.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ieogiwvm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lmnrsast.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3skrsakqb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rfshjsed.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3taqvtcbn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3spmebwhd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ksdmcuvb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hrtlzdxg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyeciwnj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hgvpasvg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fgtxlcoc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fzjghiis.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tgmlepsr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bjttelsm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3iqdwqaec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tvjamlvx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ajyqddwa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fuqbrqui.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qguexdpu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bvmncsvk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlwdcpdt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ymfsmjlz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrfzfbrw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mzwbygvb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ccomfnri.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rkxixawy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxfcbopm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xemzuyvk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3defzbqmy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdaekefa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogpqfswk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gxxbwxvo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3soxxhjsu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cetmgitr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3faszgijl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3alycibaw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3vznaiovn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3legrdbhh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3etxunieo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vpisaihn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cfgwvbqp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gmmlhhuf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tvfsxwkc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ylbmwvzl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3behfpjjb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3preyalfh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3aubjyhjx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3knahvedj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hinfshhw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jphfchpl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdgzvkdc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrrspfk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zlejzrof.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pcoezwhy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lezllrkp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kqmhnhhm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bsioutxd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jnbnujfn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mavunkjk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3baretqgd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlnckce.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fdwjamxz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kkemetyz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3eguwpsjh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dflzgyld.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zhzbocel.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ugtfduab.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vyykuike.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3plbmtipi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3iwnfpvru.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fpgvjqxf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wfxtzsvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpvxnexo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xkbwkbtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yirxeedw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vzlyiowm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xvtbeebh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhxnkvl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jgrsmcch.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dsqkwvsj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpueyjql.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ayffovut.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rasnqesu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmktumud.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ewvwkekh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mxqjvttr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3raxofocc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fkuuciwe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3llwrmsvx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xumeqlns.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3feujowft.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ytdbbobs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zexnmggr.html


<!-- 参考信息 -->