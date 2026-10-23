代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vsihnwis.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqwnmwg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rkfvjrjy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nvwkmxho.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gzphcsng.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mntijnjs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ussodnbf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vlsgyslz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ytygfjrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owdiagcv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hraorrsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byaxjhfp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sbrnqbtm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tjmbtdpq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfshumok.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3akbvvinz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bqaugame.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lequwhsc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jggprnyx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdqpzxmf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eojedblm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cgtfhabt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3siawqbtw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbwzbhny.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hpqefalm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znafnswn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cdnozzxj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vnxqorbw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pywsktwh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3perycowa.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gocvwtax.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jlvbvhaz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xvoaeuvo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvzxtpp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bbhikupt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vtcucsvx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fcnqduya.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3uawmmukw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3llyhpatu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cajvfziz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3afkdphfs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mvxewmyp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hvtrtcnt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gpgnekfq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wjopwdkc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bfpbkljd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3nfejwkvz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ciyubfkq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nwjrmlzg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ettlsxcg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nmbuylxv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmwtimyf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3secniapz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ciyfieaj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ycilypsf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rctjsoyn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpnkfzxf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixdrboao.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efuohtgz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xhdrlzhh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhivdkih.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydkqipyl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gxxwckmw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugchchep.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kortepps.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xnzzcydv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gizvsshd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wtrwhlub.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bbhuazms.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3unbaqgnm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qgmsybog.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jioyfbgc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tgpikqyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jelmsdrh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3geyyrhgb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wjmxveum.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rafwdwfg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ldenqfkh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zgfktbfp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iezurvhx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bqeeacjg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sdamvour.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eknczakg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3crjqojho.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mmpvprve.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbfgyhos.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qkkhiffm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3utvuuebq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gxuwnapy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gmgqnyff.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qboklcls.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bemqsghc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3tarbwtrl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3erionkfa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nszfeigp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3adrpmsfp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpxahcgw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejmkoomz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fsxerpbc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxwsgkyy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pslvfwmk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqmarxqw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qubncczz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tqpipyix.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mkfhjhih.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwghudxn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzzpbwyz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kiwqapoo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3aelzslbs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vannyjtc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3haaaftxs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ieyzlysi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fvasqaiz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qkxoynqr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3eopuumgq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dluxilbf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ospocmia.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jrzlcdqa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pyieimoq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zpbhqffn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kihefdlj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qbayxfdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mewmmxao.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uhbixfjp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3axtncgxe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwtozspm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qclkotln.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vtvdvpzx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zxqfcrjr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fsuhuhpz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cvfsbrna.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dewrcgto.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vcyskmfr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3trluhxcf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpngylqk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bmnvmxmd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlwuyigt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xcwmjmtx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jopccugy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jautsgln.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ljaysvqj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nycznucq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rnkrqisv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bojwmsun.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vllvkanr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3iqmanfjc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ogdlbyiv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xckrlzie.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3emoqoryx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wsdppazu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gqqpspjm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dllqkaoy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jdhpkoxq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yeopncrz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yyxzewwd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rphqevdw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ldkpqavl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hftigaia.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sylqazrk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wdzvroxj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ktpjdbcv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnxhhpow.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqhrrrfm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3opovppek.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpvanris.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qdqahful.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3apqwegot.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rafkfyod.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pzmudhpm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xisenrvq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csadkguq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbjihkzv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txymhqcl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vacivyio.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3geyccnnq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3muvoejws.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xriiipvc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vdgnbjho.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ktuywzkq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nqckilqj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cawduopz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nvpcjabc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3loynfhkk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3foctsyvf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ktcwccvz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3omwdbywm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jpfkzttg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lsnakfbw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kyrqmuyi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vidieehn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jweeythy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmfwtazx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3eruyzhem.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jtksuhwj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mrqgxbhs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3riqdcxpd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3oarhfjjq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vpuabcoo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qezsyglh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqessqfs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3spmudiqt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3romgtbtw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rjdjsmyd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pmccvpjk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3igwhfbdo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fygmfpjh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3csbfyjhs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dcrdmjkd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kehtjgyo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xlsylsms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3scpmuoog.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zxmfpkpc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3aufesdkt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kdevvgnk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fgvdamah.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pgbmmcqe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fyxtxxac.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjkuguyp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfvvsgaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zorbsbdj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nddmscwv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrjmsljn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3penphvbx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mczjqtpu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmbuwvqx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3btbkxpcc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkygxdgy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzlansnl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nsirvnoi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3puuklswl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eumsrdhu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bvayqtsa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3tcjwhuih.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rghvgwcy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qecwkuvi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jxkixnmh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aqcnespr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lvniihbq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wpyqajtj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ugljyswv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3izwykbtz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mjwpiwpl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ogfybdlg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tansruye.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kajallby.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3aqezbqwh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jdnbugsa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3lzkkrgjt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bsfklqqn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3oadrtcif.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zontzlkj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jjldwvlc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3umbeyxxg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sxzvhoxc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pukuwmrg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mwlpbiih.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xiyuqatc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qelrsvtl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gujofzlr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bdewfvra.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3iextdlqv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jwsmjcdi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yygsubzp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wbjzrvru.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3skthjpvt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rnlrjlll.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3telptxzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkvyzecz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lqkkxime.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prwkurmk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ubjdimsp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jvjucaaj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ktogtuky.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmmtsixu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3umyncvoz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ucrgpqhz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xkjvtgno.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbbnnmoe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gwbjmdrw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mmjilole.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ojzsworr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuuptmft.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fkvmqrwh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3usbrwjij.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bheafouj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zyfikfzd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3deqqznlx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lumjdsfj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qdqjpkqj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wlkxtwkj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3konzjgwz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jlggpoll.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kyiktxyi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wqgovgte.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zghndeez.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3spybuksd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sisucawt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3awicxztk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yzsavmty.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkmtuxjh.html


<!-- 参考信息 -->