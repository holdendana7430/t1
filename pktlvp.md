代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wkxczvnr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3furgkfam.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3txnijbdn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3smjhnuij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nxckqxal.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cpiegzux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3krufkmoz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3prbtqocw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nbhesadg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwugwypz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rcenxvcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pijflweu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgxbywnh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mrcxevtw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3objptmmt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bomxovqg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sipzejcn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rrtwgnqc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ljhaacjx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgthzrtm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3krvmpajv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3luecizep.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ekpmmbml.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwcftdmv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nnhcwdbc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3reqthkpa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yhvnecch.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rtxuzofw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bdcpknwv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zyftlazt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ccqoormz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3krktphin.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3usiqmelo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hsarduyb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wwhaksfg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kuepuulk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hwhbctmr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cophdndr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3becjolju.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3dgokzjlh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gncjrjvp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3vdirawas.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oqbokrlw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sdrdebqd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dvaplcjj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zmlevptq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lslappqm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oraosmgp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3adxycjgd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dgjpftsk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rhfcdhom.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohwkwqej.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxoqdcuj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ujatzskv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zzgthuvu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpjirllp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzmbkmhu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gftlhpax.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzawvjbr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zvfgtkdb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejpdbtcw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uoxqyaep.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fduaauhv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjxctthj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vycohvoe.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ysnwlhnz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3aohlwgwm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jvfoccde.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vfrgowau.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fymwmlab.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fgpetgqw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfpvlcbk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgbkriy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xnvapjdo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wkzqkzyu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mctztjdy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yhyovuls.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tvwvnxeo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mixwxnju.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oysrohsf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xabohflg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tcnhegmm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bofosgrm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mwsiujxh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yyoocgdn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vrgypzqj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jbduqsiz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tatvunqn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rtelqtmd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rlojmzyc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jzlkkzzy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upichdpa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gxsfvlfp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mjufhwtx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwdekbxd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vsnsedjt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpdmdhjv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3glnkexca.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wvhcvdnd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aeidklyd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3trtgswvd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efmujtmd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jaebxvdj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tihhtfzu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oxsdxxct.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svewfywq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqwyudcy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fwybityf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nrcjvwyw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swhxonta.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3knbbthgj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mixuttnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pszfbykp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qspfvdyv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jgksgrvz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bmhnbbsq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lnvkxrbw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ruunnshz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xjbcimzu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pdkoidcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njsvzszm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jqybrqpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nesmthds.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wrpiadnk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3amiilwan.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hiwsemdl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjzqkdws.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtscylee.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lulntdvy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdvnxxf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3iejtygcu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxxljoxn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zjdwrrkc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tcgwzeoz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqlbclph.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmjqmksf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wuehqynv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xldpcqpr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3txlrqqtu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqdoxzye.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cmcvsijt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zijfdffd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mnqrwyxw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jxojpirz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hdzclcbh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bcvmcgsg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3poqpnibh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uftuyklp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3avmvftsi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ekxcolkp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rtmcjlfd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ttlsqyvw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jctamsnb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ypaubxfg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmcevzpu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpeamzxl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zsrruufv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dvhcbbiw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bnmapzip.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jpbwgtvl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wjplwgkx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3niqslqls.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pkxuhnig.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fzdayjrv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zevupfga.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ivtdfgyh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rzkxbslt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pzzgukpd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yfhcpnom.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wyndquyg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pweeoyhj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybzdokqb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlfigsmj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxbpvlkh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kptgyzqm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjoyqfun.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ympsdbxb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jmmrjygh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sdybmwig.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hisunobs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kojiwvqv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nzjzmini.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qbziucdg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wiphqjbf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3esozbbmc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xyxjficp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rpdqbvrf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qukjejag.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3galxxfug.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytgzopaw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3geknsvfx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxhmaplt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qfdjecfp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3erdaeqvo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikncfjiu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3aueqmcun.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3htdvwyyt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qrhfjlaz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3quqfsjkw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nenkjmxt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wpdsdywz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3sqcrlmda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3obrjodum.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3holpfppr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xncoujyt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bhrluaai.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3piggbuna.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3iemypnmp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eaqisqnp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iuetmqxt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3igowojqz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sgocyqah.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3frkyburf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ypucwwoe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lmvygfkm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3joizqngj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuofgmxa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3obdgazbu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xlxmzfir.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vqdfiwvq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fvjrwxgm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xcaqyyje.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3exjlppzv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3minafxvt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3apzpqlec.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3shgblhtz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3feeazdqq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tdolrrge.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ukbvysgo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3moglqbga.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dlgtzmqj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3iiqwpzfv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nzyshwxf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3udovmbeb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vorfwnvy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jfrwfawl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ayozryav.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3dmlexaro.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kbufqrua.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fiviaifq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3heampurf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xlhwawwl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qesrpefw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vyubweks.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pnqsdgrt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qtscramp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zfzgutcu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hgolzjon.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kaedcqty.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3etxgnqws.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iuglnkpb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3weahjwdc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xyaujalb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zbndalmm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3npklunkf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3naeqavbs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xyylfhju.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zpthokll.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3einpgybm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lclkbiyl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ptjgyshz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kuxpikid.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uifssfum.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nmnhcqpp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cloozcpu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3oilrlayv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dquyesjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbfcmenh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jpmfafzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyvxpdfj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ezdwibwk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vrkxlsxt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwfwvezf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3krjiyopp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bdckeegv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbrucfvj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eocumoui.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wyzurjsq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjxqofg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nebuvrxl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ieihtvqf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kjctkezi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kayyrogt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uytzikfk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpuxyruy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yratlnjf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ghxquwkp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3flgvferu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fmachlot.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jriobvpy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbadoqym.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aydiachi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3opovxkts.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nrxyjpkw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zmutdajk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qfagtyhi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kvjjptxg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xyugxnwb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xkduqtob.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzeuibnj.html


<!-- 参考信息 -->