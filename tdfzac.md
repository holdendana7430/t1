代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jeujkxfu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3urfkdkit.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3podbuocj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3okwcoivj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pvcrhzpn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bszrkrao.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3addiapax.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ewozwhfd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lpwndgir.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3asalpfoo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ngxlaays.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fjdhvxji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xbeprwjm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vfjqnklr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iizsbfif.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nnigdjnp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dzfajqur.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3gyagekgs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sjhaeany.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3loltafpe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3evnpxffl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zfeojgrk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rmuepaay.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nomdirrk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kinuiavv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehshkcvj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3abymerss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seljjpcd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3efsdecdw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ixgxsfch.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sgfadkvv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3viwwsqhd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bpowwhtg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lkraoacw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3enfpqbrb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqxtejcn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hmcwkdmy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3abvpytii.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3reqkbyxs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvmggwmc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwgiufkx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkcrjwqc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eprpxkzd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3whuffxmj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3idukvfri.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cpwyozap.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xddxayna.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3cslyvsqu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cebuzetb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3npgvcrnx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3roqrelwd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bklmboyw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fcqmoglr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ldbeqbgl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wavdwelx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dnhjoctp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kobijccr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ouqxhjms.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hwzgnxom.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vjddjgtn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjdpzol.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bogdvvaq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pnmybtyb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3avgyvuoe.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3reerszlj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vgzebrzk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3foeusaym.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvfduqml.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfcmbwpy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3geqaludg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjwwevz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pajkpyyc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdqyawhm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsnsfccu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhgzhfpy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uvuhixrk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oncbmbnr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnlhkivq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tbspkwlr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqrcdqwb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3heszycuj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wlfzdnxm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cvstdjxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jqffwgsx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3urtwzwjl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3amumlhpg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vozmwqwj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ttbbybnt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ealhhgmc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dlvchklc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vdagadte.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3aahdnbga.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ijygatoo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjyiwfpc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3inrvoioc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cjztjqem.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3amrlmguo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sdzuyoup.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3sgpxvmix.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dxhcmpgs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ypzpzptz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3piudtbtk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvllvrka.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rfgsbjex.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eqxcatug.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cfuvqxst.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gtyqayaj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lihhaegv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gpcbihdg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mjvhszvo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzcbemde.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3skxaidec.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3maxpjgpq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rvdeferp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yvpyboes.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oegdjprf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhsvwksx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czflcwrf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gqwscdor.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3exqievkf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3inboasdc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsbkzbll.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oweeqpli.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhmziai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sshxgawk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nghtmxyq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fysxpdoe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tiqgvrex.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3nsntkyur.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xdrhrwrh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gsxuhdjh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ngfrmrys.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3iwnopkzb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3enoxchyq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dohmefsy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vrmyepwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufnidfsk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3johxmoau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sasmwlks.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wijpynlc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rnawqwpx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3irnsiquy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3supuennw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uhzfggkg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnzwlzgs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mhnsmxft.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qdilvryi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqhzgpjw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mziycfqo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3onxpeglr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqaofnla.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ginkxzpr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3oexosvbd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqwdpxxo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vloxgrxx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zecotvox.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrefeyi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vfmlpbpg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lteycdzi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vbdrturg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pbqkydfa.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jwohafln.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gwlosclg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3srhnwmvm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hqnohidt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uaihygxe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wfyfmzwn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vjrfexht.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ifrtlohe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nveozukw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czfmgqib.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bmrneymq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mwakzpfe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fyjeplza.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wqnspcok.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bjpvsrbn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vhodlukv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvnawwkj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ekwdkzkn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lkzckfhv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfnyzhia.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zlohkfdn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pcrdmaur.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3edgswnzc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qedmkfyo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pymkmdse.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xljitfid.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxcnhkzt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekkeshou.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yoioabjs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jxfybvhe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmlxaecx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3efqavsgp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nalgjejw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iymnxvav.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rsxhhdnl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dokwbvaj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dvtbvmle.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vhfwmpta.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tdiknwri.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cpsgbeic.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cdpvxcvf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3paqnxdbq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3myinwhlo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlyraflw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zzuopfvu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqucyghy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dessyaoq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ompmmoib.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3buifyfph.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnoynywa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rbanxxmg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ynskjatr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3youethqs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cibwrqhy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jukrszsl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3upqtnboi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hwkvvekq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hlqxoycq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3sbpqgqso.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wvqyhxnb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jzpslvhv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zycfcnwk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mlyfuzbf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xoxcdvqz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mnpvygbz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lyvscrlt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nqlcvhyy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cbdjcgqg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ygxwxpvp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ahfodgub.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cdnqcdvf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3viindnpq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uucrucey.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjwnorot.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3estkruok.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3azygjsub.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3iytengyi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xvcbclan.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dxasqbwz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zecpoywo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3emltfsld.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lrdfojbq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yqxgncng.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jgagpwwb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cwonnbxe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ogaidcks.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3alkolczu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3iarwkvyu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lhqlrpjl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oikfvzte.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3umcbonrl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pqysvjoz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xybdcqyy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ynznhbwo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3atvapnpy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3eqwvebfu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yebsjvru.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3iwmhcrek.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nvwqeuyu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3btceieya.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pgvpjbhs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gabcxrqd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uffwboky.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mrealkak.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wubibtit.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rqfnjvgg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3yogosymk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kmiwcuws.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zqlssqdr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bfvqimec.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fpcotshb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xujkmyzi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uedbklwk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zplnpffx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3netkzlce.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ulzdkwjs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpsvigfe.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ncpzwxpp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rrpabfvu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3owawlvvp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lthujpkc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zdnyrcxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkbdmoob.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tiicglax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byfftbmu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jvzacgku.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rxrbyaad.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gucjsrqs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbkrdcxx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sxrvrjcb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxxfueh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xdyzjuyy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3updlsgwx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qmdietoz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vujoneuu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xpldbyyq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sknvdcaa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nqlgsskd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jogzbtoe.html


<!-- 参考信息 -->