代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3iybjncxw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3elolqvcq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrhwywyi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3seottbes.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3tjdburhg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zutmbtah.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ljtsgjvm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dtdbrqek.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yvnpsazv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qhzfhwdc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zvbomjdo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3neomwzsl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3igjxiqab.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqbsmrkj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cnrggjni.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xuieeqev.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ufpqoziv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jjcdjqgk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xffjjznt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vbmixnmm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jlscxubt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkwzrpoe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wuzfhlph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xesonanw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dzbtpffp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kctmvfqa.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tguxrcfr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vhfzsroa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fecotuzs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dhpblvbg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vwqrwxsc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yswrzvyy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pgelajek.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3crsyinzj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3snzacgzu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wiyglwki.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgbnutyg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jczjuauz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vmjryuac.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jfaxisiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rxhexxsy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3irdfmkmz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ptqlhbvr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ricttjqv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vegtjetm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3foavxnta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3moheqbrx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lmydrftl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lzbowhyf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pbefvaic.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pbsgwbtr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jgjgrpgi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wxoxnytz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ualnkwwn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zgzjyitn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kzapgouy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nxjqjxnu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3igovfzcv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ebtyjxqs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iqshjivb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ofblwwor.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ahsbxhhp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cyjmfnmd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbifnaoq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qudpnmmi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3whotacdq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tgszhfsi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzcviutl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xosvhpag.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jbhbilse.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qeqhworm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybswkxmn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ockyeeth.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxfplgdr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fsuezmgt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fsolktfm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnmbmstx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khhyerei.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xafyhqma.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gqztejpp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yxavgayr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ucygvekb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kdrwxrel.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ylbdzhej.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xduhwahx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dmzmkuxc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bvlcxkao.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wdhbpngk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3enqcytmr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kugpxlgg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ufbpandp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ckhyblfe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ezlzcmfc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bphjvhaj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yqapmljf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gddvfbzp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dqneomyu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owcuafzw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3waeceiwi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tbhxkhoz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zcyjxuau.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cthccfio.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kcdbutri.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsucvzju.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ptkqvnyy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ljmafqhl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shptsnkk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vczcisdv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kftmigdm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3buedbmtk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3njehwmkd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3noqtliik.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jocicyhn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3saowioif.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pruslxta.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzwfbbik.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pvjomztf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uedrprsj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxdyqbhk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zwlhptnb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ykkajfcx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3biflklpi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dlfgsuct.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jvbeyjpx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ouopxnxt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ceimxgpx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rwbiygzl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bthmpqwc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3tbvxwatz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jktyqhjq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ldidaxlj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xjytkaxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwarvdfn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3poehfsft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdayimoc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fjqjhmrr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3teekkwoi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tjckcgiu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3saxyjkia.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3soqfgwno.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzhcgjxl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gpvzoxjq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pazbhlxj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytyuonme.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vrcqmrov.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3eayxchpw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3icadkpjh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpvohtyv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3besqzvcf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itfuvxaa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3lpsnckcy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yqozycrs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sfnlctwp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mjbndviy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mfoyyozs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3scuqxamf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ciyexcti.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qgijvbzc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bwucqisj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tockasck.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rwaerooj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lcvruoxu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ipkveari.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gvelxslj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3saygsidt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3urrxbcwl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nxfzamph.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bachfsdo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vcyofkoy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3inqqcpyy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3khwuxzoe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kykdmbke.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kbatoytd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pojqfrsh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cdhbxnvs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sicrjzfg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3asdiwttm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ydryldhs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ydpxlkrd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hnsqkpdv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3oiqidfmj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3efdyvuih.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbeljmcc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sccgxqhf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vcwspvdr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nczrzrpc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3esjaemam.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3aunkqtpw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dgnxowwx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3thsnorhk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ifjuvweo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ocjgkbpa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qkvfdqrw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wafynord.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hhuqjhaj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pakvsphj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ofjpluan.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3aawadvxx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ogitkgam.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zqcaqgzd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozglimyq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsrvorpz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tbsreoju.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ptnsqwmy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ijizoyip.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3eccitcfn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lmbocvez.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3sdsgozgu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gcojofre.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3arnxyzkj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ybqhasuc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubofksts.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lroknenk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wbqaovnz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fejrtgri.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pklywfcc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lxysdskn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hhmxymkj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mbvcnwyn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rfcccxjw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xmdgzilk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3spczkzpm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bfbejkln.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bkfowdmi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3irmxhreb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3eiuggejs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3amtfcgcp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mtjnavfz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ciznyecu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwrsiyzg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sebrrxuv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqmkjje.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wgcxfpxl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ddlwumow.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ffichdih.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kjcgqcvk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtplpul.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znpozjox.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzvwjhed.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jjekrvvy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3prmntvyw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kocdqhuo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3skrqjyvg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdieuovv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uzapshqa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3awzzxtqd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uloswdeg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qqdgtaqx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wowpzipg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3csoomssr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kafjxvwd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3amelvkic.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mlxkqyrc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ipaenkyt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gqqfhdwj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rvkwyesz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tdouzhum.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3svwiojzz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3imkivgdw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ffudtaeo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vroefxdo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ciohlnxe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xfchiung.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3eqzveupr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ohkhmnqf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xsiojdow.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ynicefoo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3kdropaoo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3akilijob.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3majusbsg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xanwerby.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hpbeogzp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bpuwhzvi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tgwyowoh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evgidzup.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fcmeupav.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3dqztuvuk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zvqtiyut.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nytcwnnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbfufqgi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3obfetnhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzjnvmgr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3grjovedy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kroqkhny.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3urwzmdod.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ejspyspn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdlzpgis.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yqsfsvlh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3csqwfypb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3iriedfnw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbaxdkps.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xvniydgi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mtlpssbe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3veifgnps.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvwjtogh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnwveyin.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xgfxvywx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3twoxizfj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fhazuscb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yksbboic.html


<!-- 参考信息 -->