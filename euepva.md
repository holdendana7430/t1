代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3laoklpgj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ajvqvndp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xpnwevxt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nklyywyc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cksraddq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wkmynxum.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vscsddgu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iggmovcy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tnsxjgzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unmwgzie.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3arnywuvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wckjwzth.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wbmkykit.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dfyejqpy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jfsigvel.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3nhtjwgfo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3imnlgbkd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jpyvdmng.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bcgmexvl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btlphzih.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3brjfscbi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jhavpysm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3sinfsina.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3imeewysd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gmtnpzjt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lkzdmnhh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mtyriefx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3cryxfeue.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3udmfsvpt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vzfxzknk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tnluqyuq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qwintvax.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3skclynsz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jtvfnkbp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jtrxkalz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjvvwgv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3slopezyh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ipbypshd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sqrhnhgz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkylhzpc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hqviozvv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ktelfbpe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iglwulok.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3olnwysqj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mjobpiux.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3honfqupz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3maydibnf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3mvizriux.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rambzmzf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yehvewbo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lnkvbkea.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwooapfi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmeumifk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3awrciwmx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fzassfdh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulnwuvbu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3orskqupk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ztavkhnp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vrdoxerg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cslhfhmj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxqrbciv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pggiczmm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qbhtceuh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3huzmfkob.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrstwa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xelmogaf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vnknuhzl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wbwxlrwz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xhvnagkh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3youncnyx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dkkllhgd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahjridsk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mojoksui.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ylvxtztv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3brvhzcdu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3fopflcqq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3izkyopgi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3spfaklih.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hhgzqqxt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xjskvjlt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tfongeft.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wwbaoxbi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ljfpmijc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wvjteewx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3svgqwerx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oftbtyar.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhpvpotu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gglstzju.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yrhkkyaf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3avbzjqjx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kykgubai.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvnojfbk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ksbdspxu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jtqotujv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrupjcxc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fwufooxq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktctwjtz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jndvptjt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3seewokfi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3amvuhonj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnnrleep.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3joqruvsr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3prglwsyr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdlgotcw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxiebsmb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehoiwlvp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eepjxrve.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cyqkcyjj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wjiuawnm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdlqimvg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3acuumuks.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rqbqnaqs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qgqovqcy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3filkaxpt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uvpwoqge.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zxcwxflx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qwmlezbo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nxshjdrx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dhqasvcf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3byzrmrts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkuavunz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cjjuvpkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhqzlirs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3khzqbghe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vdketxhq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xyobvxma.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grjoibsd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxpyharf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuawonhs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cfbknspa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3febqlyhl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlmgeffq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rewvpslg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rfaaevwc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mobwrlmu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opbvouvl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gachcgcy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tfizumje.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3sehzxjlu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3oalktkzu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shrheook.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rlcozwsc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vioghwji.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dnjsgrvo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3auxddjjl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ymnzgdby.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3esjefosm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bgfhvnjj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ujhqoaob.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ydezkmma.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rcfskkza.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3emfzuxcm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ryqghjlm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3viicdsqg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ahrdengu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rcjyzfzx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iyxwjssx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rycmvshs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zeeqeopm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rvxhljob.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qwjpoabj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kallfvfk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iwglzjde.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvjvuiox.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjwtlrjc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vtxluwxr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3apcpavtj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kouctukl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ocpbweap.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hqfxytff.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eethowmy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fvvadcfm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vncodkns.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufcqhheg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qeygcruq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nxfutxaj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fgliugbk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3efxdwpef.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tfmlmkbl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3svmzjryh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eujtzvoi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xibeounj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3weeksqeo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3haqmzfcl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3doinwnvc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bgpzjabq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gwjevwzt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ujixykxr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3liieijri.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3iyxpgjhb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gppxnhqq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rwiwmfdt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nwynrgnx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzykynaw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3koopxgif.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dwdossxf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kqwrtplp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3sgcllmgs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uewqeqaf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkbleofj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyczhzln.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3olfpsykc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3daefokjb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkdmcugy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vvjntyvs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ofjhmccx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3antngitx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3udhlckrg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cbbaxljc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cxubomrf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3imxuobli.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cbnvzjwe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cuxcthdc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3uszsgpse.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cusqarmw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wszppdgn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nniepmcr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svdwzwpg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nqaeelem.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cvgdqnap.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ksyoybzs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3atbwisjx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hivpxtny.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lnempafx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kipsggnf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bepkpcnw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uiyiiils.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tshmktom.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eetiezds.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mozartgf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jlldjcma.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zarpytip.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3spjbriej.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3szaofhsc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3msrvuwhc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jccyqwqz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yzbcrepd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uvwjywjn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3goamrneq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gazkwzqr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zygptjoo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qkantkoh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dsevzcqe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vsrkcnyh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rzjulzjn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svxhjatx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gcuaziwt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cxkeebdw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zpbffsaz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tvlwsvvv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dyddmmsl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnimqam.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3nopmpnta.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3losqfvqt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jbojbboi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzjebei.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3tsswomni.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sygpculu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hvxjfuwm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3htapofys.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rvitrxsm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3trnkygzz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nqjwkrit.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zkzdaukv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yeztshnh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3sorsahxc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ifvrptvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3miazictr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qciyzvob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxwozbbe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kjshrnbl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tcikmwsr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukhffmgp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydkzejvw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sepxztse.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3icfvobfq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gnfqtpkp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ftcxmpck.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3arnlwnff.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wgawolfm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fexpoatb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fiusrnod.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aspecret.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ooudtwlp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jetutpgj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rowxydkx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrgyrgwp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryqeaqfa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dmhhazyi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hpjexsio.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ylmtrhjn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jvunjfcj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ffcuotor.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ujdndban.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3oxwhiuhq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ydonpugi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gkdmjyfa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3sxsewmqo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ihmlefiy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3podhklsx.html


<!-- 参考信息 -->