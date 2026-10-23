代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uqdbmhzh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pgwduklw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nxjlbzxg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3guxrzfla.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tppvdflm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfwrigay.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dpqqgcfp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3caknrzrp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ujkfpwzw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ouazuyzt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3pfhdmeko.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rgtwhyqa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cxqsgmzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvupnkpg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3tsdkwucn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnjncxes.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yxjztiuc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uojybrvx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxitzjkb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ydsriqxk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wwvjhccj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjcnbpgv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pbfuxxbo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhuiskg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bsdzermm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3thihibcr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3arynlqcu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3drrhtjsr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3egwmrxax.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3meecipxd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qjiynvlb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rfqjgmie.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mkxqtcns.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ekhjqlru.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3luidttwd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3edhaspul.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ijauglsg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vlsutukx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zjenvyjg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rwiqqbfa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ptslhldh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3aqvavthl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uojodkog.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzrzgbai.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zburosdl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dsoujoim.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3soggcski.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sprcpakj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bdaqoyht.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vigsukuf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3oqbuadwa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3savbcdyb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hamufmeh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hpkyvtrc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rdzlkplp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osaefsbu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqfdluka.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ohkpzoik.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3eccznypt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ooefrpbh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddwmcziz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3eqtevjsq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyjftvmz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jwnyixdg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhhewpaa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddlhsuuo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yokfywzg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcbckzgg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdkbpixq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gxpghusm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ukikvqva.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdzjrfb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ujfwkazo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3szsujbix.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rwdppymv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bcqlshcc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tzflihvi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3brepduke.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zpxxnahb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vngujnks.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mdbxzvtj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ekgzdajq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iormipiy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3acaayvmc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jqtsefti.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ecscgijr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qizvcmvt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ozjpzygv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kviteqru.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlpbckqk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ahcrhnbi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rplunauw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xqmswdju.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pglxatbt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wcszdcyr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfxcyazo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uqdftjqm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lwkcxasn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqzrxzva.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqcfqvvx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwtjpjga.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzaopsma.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3phewwdzo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aextvpzy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeibvcdb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ughthmqo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlqkpupu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqtrtbec.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mtywnefk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpwcfuob.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xzjwfgws.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dznmbldl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qiolzvgn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3huarzjph.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tvsadfyc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dascnprt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsajkuy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dmrrudyn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nsukfxii.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fygwnkkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3aywvjmwa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ccaevpgh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bdhqkote.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ebijmxps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtcovzuv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zwejhlpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcrzlfsy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3oonztrhy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3naoftmke.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3euybhwrc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dksfyqxi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wofqvfsc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwizemtl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ltytxpft.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lfwvgffs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyltgjwb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3owzwbbpm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ptvqobar.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dnbnrjye.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ydgntwty.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpgikuyg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3avdajhvc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nmiaaoqh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qubwgrba.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zxjsmhkh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zjgrwhum.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bwrzouqo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yfxsbsfc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3stwmrgpo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nljthpyg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vvmmevub.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3adxxghxx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3usclessi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wzmpsoey.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lrhfoccs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gictnpdq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyjkbqdm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dtfzetip.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nzuchubx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vvpiqejb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjzjlfi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xyfcwlus.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3udxfftdl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3plkmrvki.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jpnwjlmg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mqqkodpn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vauouzrk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gycksuwz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvyhirfn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wfgqnvqg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aoejqckx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ulabkdko.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3igsorjxf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3icinlqck.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsqcedbl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oybgmcpv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmnikjlw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqkpcgqy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cvoxkhhb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqxjateo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tresbvpv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rmvufeyy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fcrsmsdy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kzhspoyo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yhhtsstg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gsmsvveo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bgrgtxsj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jehjnflp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lbbkpdtb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zhkkhuoq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pjrnefjj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3occugjze.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uzobkprc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wefsrgen.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zzowkgbl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gasjcjzu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3oitjkryw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ulybsynw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvurater.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pyrhudbi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ujklpqfa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3unoyfqkm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dalgjyrf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3txudztai.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yafimikq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dturnweu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xbbevvwu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3giocznvn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3boiybsri.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3mlxezuvt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mpdonjzi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zqloqdst.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ehcgfxuv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3laaxvpwt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3chfnywun.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pceocgew.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vgfytfyv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3laaikyjj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wqzhdcox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkkbhabp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyemdahb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xrmhnmhp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vfvgpmxo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rtjbrakp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fqefccho.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyuwsaai.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hpbxvapo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3veyrxslk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wddzqmzt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zjkxypdq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyzkixwu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cwnqinws.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vntmvrll.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pwtoxuix.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nnoswpvg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qhusugvq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cplcjsvw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3grneemsd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fsffuhuh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zollglil.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3awivpzol.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wmajhddj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vgeoitou.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3cgtugoqe.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3blclntis.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ufjnnlfg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tqmcbuhn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pzmkxyry.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3yiuoeecd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3encejmyu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bwnzyxbz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qexwfmeq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nhcaiqwi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jdupzmtp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvnjztle.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxpcrhrx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3onlmygxv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pibsrzbs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tlnlnvcx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ortmxlhi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yxswouli.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sudyllcp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3csokhqga.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jwzprxai.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qdywmsap.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixvrlaag.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qphbvsjl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qclqzrbm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tbxkmxqx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wumcfhca.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ijciqpmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkvzrgrp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3awasgfyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmmndgvt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3szsictot.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3obztfvrx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fnxttmzp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3owppnsut.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ojschnhx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3bdoiqenv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hvfuhrju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qtfultbf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qiyevbdi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mrpiywko.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3cuwedfum.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3izevytdu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3raxogfga.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yqjqxdtu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lajhwbht.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ljywtktx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3idlomxvh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3luysayxa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kdkfjkcy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3adbxwefj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mgzpqnsc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yywqiylz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ldolhpnb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zftulpik.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nkolqesx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3puuvgbic.html


<!-- 参考信息 -->