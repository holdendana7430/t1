代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ovmourld.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ldngwmfd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nnpddkip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2whbtjnbs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pwgomtfj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2tyacsnvx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nnsobhpe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nkyyzlew.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2frstmibi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ejfiupad.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zqmsfwwk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ottargmt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ijdgtwpq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yaksegzg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wjlgcjwq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pbzxrxjs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mslevtuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2exnsrclc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bewskeej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hcvmokgx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lltmixhx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hmlfkqpc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fgszotho.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hfevuxbk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wcpuaprm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eaktjaim.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uyowogrk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wajjxynv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbocomcg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2iphaiqpo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dhjyrswf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qbyiwcgj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pqifzula.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxyrlokx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bbelljzu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ceiplyjh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jdkangkd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fbgmgraw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tqwkobbb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2epbhumrj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ckkmdlmp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pttnutij.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2allyzrrf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mqbxgljl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wsudszto.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dctqdevy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hjzhkedd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2crjjxsxn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uoreikqj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zkmcxeoh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wwukpfdd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hzpdeekr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2pkcytrev.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2frexqhqh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2oktfzsaj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ebwyudba.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2clbscrnl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gziktzix.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbswgiid.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qtvtsayu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlsbordz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ryvxlyzg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hxyccrej.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgxtjvwy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrsjabin.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jmrycakh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wotbdaod.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2elorpnkc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aunyqshz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjsuytiv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2swijyzgs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lyzvzddy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdgrcztx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nnerbbbs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bcrrqrsh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qgmhuyid.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lszjaaap.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uvrmtwoc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sbihjqvo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wbiytlsw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uycbzbwy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fobhmbtf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xywcnaul.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bjxrbiow.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ogzshjmo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bdmfojaz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ujstdtgv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kfffffvz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hejdjtnb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cfhtzkki.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wfndvuja.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ynnnfght.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zqnovqlt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvqkxsut.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uwdebeac.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xvypwewy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sjqjeljh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eejdqhgr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fnjlhrnb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpnxgrup.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qmysflbq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hgdootwp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htxymuub.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wefaoiku.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xspvxkui.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okurcwfm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2owkhsyhj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tarhjeyi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgneegop.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mkbdihxc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gnppfsra.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuotnqfi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jxevrjld.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxrkhvkf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uskjbpjq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lnqvyosb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jsslcbma.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecpmiruv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qfmmktst.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hsvaguao.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jmyypfsx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gvkiqixb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2soowpwkq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ukutnwbf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nxfndnic.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dwsflpdz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lokxxjph.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tlvwsrmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pydshgyt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uypvkvgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgchvkux.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cnrjiurh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gaifzeem.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2uqxfasfp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzohjduy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtnozikv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcrpihps.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2siwbphwd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lxafasel.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jdovjtvq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmuxpink.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ihzixxzt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lpdvzjag.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwlomofa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssrjhvmz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xqocigbb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hzgcofep.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2beuujnbf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghnszuyj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xpjenzyd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gxehhvzw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kyysakax.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sbaqfoqz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ehzvehqg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vzxgoijy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ufwzedme.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zvxjrlxy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jthldemo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ggdemgyn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yhnufjul.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vocfjiee.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kxhecoun.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqwiziei.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkonnipq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2agbymzap.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2toegetcj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dnzxpzqf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tasxdyte.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2srxbvlvr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vtflsdpw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hbkpxudv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ishhkjdw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gorqirwz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wzkydvvz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cnctyaap.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nzlmkbaa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ypcwftlu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2yvjwwbpw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebrivlov.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbjylfqh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmvwpkf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhjxyfge.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fvoarxim.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrcnxgyv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kzsvywve.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qraeetsv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nqllwpkr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aeldsjdt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jonacnrc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ugnysrbc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dadbdqvy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rweycydv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ycnfodvt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2omwafdrd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bfrdonno.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bpcpwlzq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vqcdagaw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hxmjmhhs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2orkldkgy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2dofwajlo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vmymnxze.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zjjkkohj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2buwqkruh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sgpwbxle.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qclavrjn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjvlpprn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lwhtmgcd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2aypzhbje.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbblsmou.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2maikjqkl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rwkaemus.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqyepwwb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ytifstji.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2arzchiat.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vbytendg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xebumjro.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2damofnsk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2umjmjywo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2yszavwxp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hwygduom.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2crxvgmiv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2whwnskqt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yicjvspz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfexajkv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ykosngup.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hahywgvj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ngcqzydl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kodvzovn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2oluntgch.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bofzhsep.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwwuqcjn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ypmamlsu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gnkwzbbx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knckzkzf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcbroxzr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mbtltjyp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ttsmxtuy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lwjkpxus.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cyqvedpv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wkkhptjv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wdadljwm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tqkjtqhp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2teozwjig.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2japncjug.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2btclzqva.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kxojwpuc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpfzeru.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2yxmxyxlu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2oqddvzyc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ppwwhkwb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zameucdw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2byacxngj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mqjhwztl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sktyuday.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2juxbjbyq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jhlknmrb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ezscxxou.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qoraltbz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eokmypew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzvsfvwj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2obgniejg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2drivrnbc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ljkofctg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qqxlynns.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2vfwrpbnh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jyguhqgz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2janscdda.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jepmtjmh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wlqqlgvj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2praqpcgp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2evtkbxgk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xsgpoqgb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mhjtqtfl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2unwrspwr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jrlnieeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osazkqhy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kuvbthto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2soallsun.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zhddncwq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lnwfldur.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2caujgjls.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vynmznuq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yoqlnwez.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekajbxcq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fabvescc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hldezixf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ctfxuhkk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jivnbcmd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jugfzhgg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2quelevql.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkwctkoe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzwohhtf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyfqxpil.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2spqkusgo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jxwekiop.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ltlhwhbx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rejizumm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ifppntuh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wbfdcqih.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lxxbaont.html


<!-- 参考信息 -->