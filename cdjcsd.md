代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3orskkgkl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rgevrvkg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xkseguyn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3smgvpvnw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dyezuwwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvdssztf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hwtpjnap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbypvsza.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3osoatmkd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3evialllc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yypdmxgp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3npahatlm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3opgtpwwi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3adbrtxlk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qxkzyksz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmhbiqtb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijvbzkpn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccerfzze.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dbvbeanb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sbqchxmq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xeztgkad.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qvmaglal.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3arbfmirw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kfmsswzm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ywubccmj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mpexjjut.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qfybhior.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hsfzjlek.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vkjfhdby.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dsmryavj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dbmzntyv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ilecqidx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwsqdhv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pcaatndn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nuvyahah.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3elcgxaun.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3utxqffnr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fmhwekrh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vihiixbq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yhaehihv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3imtnfryw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fulgisjq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ggntwxjh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eeypkldz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dzcevzpu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zgiknyfi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3deazyuja.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ssggyyve.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfvauszy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fifazflu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fwgpqjmo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yupdkjqb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3truryhio.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hoirbnfu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prkhwkkr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lynzvcic.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjuzldym.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wijtxxat.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lskyeznq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjnfdfcm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnhsebpw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wxekxghu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bozbktcg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aifqxyrl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tyjlzctq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ycnsctwy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qunauwee.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ymrjosmf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tozmidhi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3robfqqwv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3opqxfymx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ihpyqiaw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dxrpamvd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xxjmfzkk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmwxypf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fvippafl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3inzdbqks.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ewppyypx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bgbmigst.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3csytsauw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3joyqagie.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3duyxlyio.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xucvxdvz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qgavppdg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3khzkrdxq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ojaiwsmb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zbawbrrd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqmcvobo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ykoprnwg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cbbfbyau.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucujleuq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dbgqidcv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avxfsmrn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgqyhgyi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lqesqjhz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfhfkftx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nygwcjcf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlyfugrc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jnszmbtf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aaivdtym.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gobspktx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyzsvzaj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwoytscw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hemmfbel.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cwmflynl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgjhlqqf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xufrweel.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zukwhunk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dhisntgq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tzetqhmo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3eugpcwmb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cvbengse.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gikpbbtn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ezwrhfow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xffbjmhf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lzdbxiuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpsewlbm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xzqmfmwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyenrdqj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kjwpwaew.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3thvzdmgm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuwteymz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vlabpsmu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3aknsqeml.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vzbfjnia.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ofyvutap.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oobucsia.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ufxziqad.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zueqmklr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nblpexqu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntlqoref.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yplwomwz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szlmbnlg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wkfkaupb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wdgcduey.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmpsuqtn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tpfodkgs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xkbniwoe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pgjppmaw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pamogajm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zrnavrzi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xixokqiw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qtbipuuz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jaqszunb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qyallxxb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kqzkatau.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vladcneh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iwqzcfjm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gdbhogpj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mkiewwve.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlmykxp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fevpkisf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ficgiuen.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rnkqohjq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ftztmwec.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qekettvz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ignnbcdg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mhmppgor.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mehffsgf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tmrvpuni.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rmqswlhp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pevfdipq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rnlkxlbk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3beuvnduj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cnpbwkud.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ryhkqefi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kmqyfoug.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zzsddhzb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jajtbxtl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kjamfqnf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ejdbpwsh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnaaagwk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ykvjtbke.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ihosyxgj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xqqmwshz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vxowlkiq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3thhvgwks.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sxzpseng.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zwnjxwaz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qijmwiqi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hmjrzwmv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hnarngrr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yuzuwhak.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ceeesgwq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwzcykxk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zieslebr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cvkpzhlw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ingpslfl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lnyfouwp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdbntapf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gurixcow.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wvjylglk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wqfkivcq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmfmcwg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ylkllfkn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jzvuifan.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zxwjxtdj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbuaxtuu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nbcolghi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zqetsqnm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dueetpls.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nugryyyu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xylgqfhc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kixofeku.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aprxcqob.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3urljpcjq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lxyeejlf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rewtmtpv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qqsjubnd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3uxuptfyw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hoepyvrz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbrnlqiz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwjckswp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwqlchaz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aykgpjcf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cxrygfxw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3visphjsx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnubrjhs.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fmhucpgk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pwzevmvt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olfchpuy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iprnndve.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqaqlrhg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hrnnldic.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3olnkgldd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zmhjgtiq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lrhblreo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3oryccwzn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmwqlzd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3euimrpyw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ewowiblr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cbgtskht.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kgizjefz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jeknhrka.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ajslfjbd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gafrskqq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zyspbyss.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lifrpayq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ycxdcnyu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3klkueuff.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3iahfezbz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lhjywbjv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vregiczn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fltglxku.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3eqrxywoi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xkxyliow.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3myszxpty.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpiwiyzn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qxbwvsfn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bswtpefq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oenambhx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kgktmiae.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mucqegtc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zigmbrdf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yytvpodv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gelwbvxb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hhzmyuru.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jrkbfgan.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kqytdevd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dhdcjeut.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qsydqoae.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dnighagz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ilfbusvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnjhehbt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wovbmxyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmzssjej.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tfrouywn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3joawtnlw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hdxuidia.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ghuviaeu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3guxngeow.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymanlygj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ibqxljse.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uotvocdw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmbjsnlr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tmuhfgib.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3smnxkpob.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rholrgfw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3goxrwuth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxbqbikb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3asbwrvoo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jfqydmtw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mydpnyqn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pzzaertz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sfbsfpvb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mhihernl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cfszavzb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3abrvyhdp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fvathccr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gbmkvosx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vqffcfod.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qxxjfhby.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pghaowbj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zcznfbyy.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mgcxcuqu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3osllceuw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nbpsnsgs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tszlrboj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cfjkzpkq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zaruqypd.html


<!-- 参考信息 -->