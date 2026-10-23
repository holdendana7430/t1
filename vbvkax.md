代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3dvhleunq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dgctoehq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bnoftbie.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rutyewar.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mkovytsq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlejpgsx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kicqlevv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlwgvert.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ysfnidfb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bfpmdede.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3beytamid.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gjixbxhb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ictvxkat.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nxzqgeql.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sxumofgd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xltkwjlc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oeuxytqk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lztavpiw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cdtxcyoi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fjresnrf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3iqzvimrm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ptgozswy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ibdjhbjm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ovhqqygy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gvescpff.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fvoylxrl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xvqbfrgb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dxutfjiu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ypqceqll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkzzyjnz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gpwgicwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qotjismw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lckhlqfn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3auknfrzu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnhktmhm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tfuybmne.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ikatwcdf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ricacekq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qfrinaem.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3auxyaaau.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkpwsnwd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ztwvcndo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xezqnblv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iqefyfvi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjwwksep.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkxdzlnd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3smhrcyqm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bjvvnjvm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3krtwdpmh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cmdaokph.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fjsramlk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tpkocgxa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fdwpbkns.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bwuabgvq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xdnxhgao.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ljrpgzpl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jhgurymj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nhvngpsr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gdlkgplo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hegjmrnw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tbawrqri.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ovhnllvf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zagxohkz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pxldcuue.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ckarxvrp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3suagcwtb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dxulvgxw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lvamzrps.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iefultkj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zsbducho.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gejmggor.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfbrjqnn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehgggnqq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xsspbred.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3plodiopv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dchvggwm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqswcned.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mxnhjqad.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvdsghho.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzmlbvmh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3puaazeyc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uugchren.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cpcsxsur.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3givsnwgk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oynebufm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eflklxmx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3yjkfksjn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbyvdnt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mwqecjmu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bzfvadye.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3agscfbzl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pxwhopyc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cywpibmn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3dwnzkvzh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hxdrcvdf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qfouwhos.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3psyetkzg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qqgwassn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wdenbhrg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kzhstyon.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cibjkgak.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jwrgoood.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pkxwmegm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vubbmnmb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mmmvxmzf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qykbaggi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqjbmcmx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pygsiecf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3elciabfq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ovwzwrqr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vtcudabc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djorwkcf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hfdqbhmi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lmfcysvg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukxvaoem.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zsqxcmua.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxrborck.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxilgkqe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3foabzsmx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvobylqd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rogwmbxn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3laxajolq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewyqjgst.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3edjewtkh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kbjhwbux.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnjacigs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbavvxxx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3okmooaaq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vozmbsxb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnavortt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3orcqvcmx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mezmrcho.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3helvodzp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wmrnzdfb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bokdaawc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mmwzjboh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ledfernk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qkmgdqzq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nczjqihn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yrbpicci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsupodlm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3psjxyuzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygzurmft.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3npwaorri.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uuaujcxj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pnphpgii.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmibfkzb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qsgkiwdo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3awlqpfqk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xepfxmot.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jzgptjoq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wqzhlcod.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vpfqhoej.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ofathtvt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3glfwjulo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3efayjxnh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wikxypie.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3csjmhxid.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xhhihzpw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3knjyohzm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbnzqoma.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hnungmhk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3paohvsrg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cvziekxo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zmxgxtya.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wiboguao.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bsdligts.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3urfatvxr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lhhcnxnt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ifjhsveq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ggmltayn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wvqithbg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vsaajfab.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmcqiojt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgcacshw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eipbzzdr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nbsnxlyo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ynqswrgc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hhdtsxxx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hjbpgdhx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3evtczvyq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3shdasbof.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uchonsxh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxnlaaqs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fqgbpiec.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3wanduxur.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3witwllpm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmcuafzz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fqddlota.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3inirpweh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bkwkycjp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kzgagubr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3evclmyuq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ndnjihlk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3oaiiauud.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wqbgbnzj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3apvcehiz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ujccplfq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qbxpeemi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ztwywdzb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ljlwugyk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tswfsavl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mbkkmcvw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rkjkcnla.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3myokarwp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cquxawjk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gvvvsaxs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tqpxizzo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwwjxrvh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wtzklfso.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ihzjlxww.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3urxxsrte.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3clvfvdwp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vxrmxvic.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xhyfmaqr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gnourmvj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ekpcirnl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jvxuhhai.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lrnzldsp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngppbphw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zabewxlq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ovqbmnib.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3enethrlo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibettfli.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ethaopkt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gjkubaxr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ckywmslh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ikulxwsn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3unvkmsxg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wiwrqudn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3cpryamkd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ykgqwfqx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nceqjbyr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3olmxzegm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kdmuofeb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wqpmfvmq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwiawcbd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpgdwzwj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3muagytls.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3szdbvjoq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xwnrmgxv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3uipwkwvf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3isetvpya.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ggpqtjxf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlmewwyb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dkwqrdwi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxezurei.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mclgsafc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3diafiipg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhcipzop.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mydyjamq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fixraxgu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3akqczqso.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3njdgyexw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sphpafca.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hqozwmwd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mymrpljk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3twvvjxoo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bdjljoap.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zweetktx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gahtweok.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kovwmvgm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bgqyesfo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gmakedry.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cxvkxeiy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3baenoely.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qnsecikq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zfqljjch.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xxkqlqbz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mjbuedtn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gghhjpph.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtgtzhxt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bdpwhdav.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pnphtgab.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rhzvpsfp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3bzpfvjuv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3niduwaxo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwqivtq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xfarrdlv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lkvdjluw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pylptrdx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jzorubjl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yuainqdw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jtcfvlju.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3utxulram.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ayhullmj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tgknugbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osayswkf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zaoqzkdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dudookdc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ghwahjcn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3uztfjfby.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sswmwnqi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lhqjmwrv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yyzjbhya.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkuesiaq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tpfmmogk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rktvlwtj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jnlbbons.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ugjpivft.html


<!-- 参考信息 -->