代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2chuvnvet.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ozrvuanx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wijtoeav.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2abugyfbh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhwvrxme.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kfbowhvg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2csiecuco.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bvcojjwg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2knntqjak.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ohwxcizm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kmzjhypp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2faliasni.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oguvfawr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qtouckrv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zzzfsnsa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tlhojgpm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2chhxcunf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtcuwkt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fvequreu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pkydmwxm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zwuoccao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oqdmpqrt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2iolbpicb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tiigyqca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ncvsxdvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvrvdcya.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2igcszsqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuvmurgs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2azgerumx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wysjbpth.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ataozrqj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ucjuyssa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ldvsivxx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gcxubpwm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2obkoilfx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aaidwyrx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ctvtmmax.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrwxohmf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qjeqmjld.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kwtcccpg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bitdgkch.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qogajysc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vrdlopgl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vxtmfprg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mmthupyh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgklclys.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2eetnaixo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tsysnxkx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cvgviuos.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gcktrprq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ytapgmej.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fluqclqg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xruiaapu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nofnlnxl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2abxjmaph.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2odjkktsx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2thmegwhd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2djcbvcrh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zvvgyjla.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oinoxikh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fvlysmmu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uhtshbeb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2neqqvrwy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oyrenhjb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2blchiroc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hhvvmayy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2phfsifcf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsgkfigz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idhtawkf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nwsiezsv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vcbvebgc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivcwjqhe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtbxpzoq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2smdqeiwk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmsvqqjc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpolehin.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdszncsz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abqmqink.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rvzjobjh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aeqdhruv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huinlbfr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2maaecens.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zqtdvgwi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ergiewxk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tsjlpjkd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qbeismhn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bnikhrtk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ocoduesy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wnvtocaf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mewzrjoc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mcwrmgdm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wbgokwby.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pfwgkkyu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vgjfwwll.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hiecyswt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gpyntizp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rpiwgfje.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xaenavzf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iaemnvty.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2prirbnjl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2busdlcdu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adsryphy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnttbrgu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zwzxlfsn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oturfcbv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sqfxoebj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2krpidykz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lseqalht.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2iobiqajp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ijqqfmzm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owohlljy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgunlkgr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yeigschi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwgkrezw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uuhhongb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtfcsczg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kloujqsr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ieambgxp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wepqvkxb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2esixsvlx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xnyqjree.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2umziifnh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejbjsljj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tdrzeyix.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hewevjyb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vpaasmuh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2smbiprlr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gxdbvthf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2obioyhhw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rvbaeadn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ulqlkwcb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qrwhvjof.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gcsblewt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zfydvhzo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ldsvjwqm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nuxbusel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jthvckeg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jvzgjjpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bycomscf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pwgqqxxc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ddarqhlx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gjsvggux.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyjebgvj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2farmsiro.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sndimtfx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xmxodqgv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lgemymiu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aetzsnma.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rnueiihf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2asjzjfao.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pfuonepu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgglxxrc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhbuxvgu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oxcuuahc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bvivvgzf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qdyhlxnn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llsxxvti.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bniaurvc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2efnmkvdb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2auvnwmjf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jrlthiqr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nkaokwkv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jlgszwtq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uvkevebr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xpogfnte.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wuvcdxoy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zddvrgis.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sbdemvwm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eveuyzze.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2unspxcfq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hclsuyyc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ejkevfqf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xuhsijkp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlkqkpli.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bkqndboe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2idzhlzgk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qgusvomd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcihemia.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fjeapkrs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbnpbbcm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2izdmqnvk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vfezdtxm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ywvthhlz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zcjnaqlj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kympamkg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gmjdzwcc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lopesnxm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oybxktzq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aernbgoc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ztowdwgf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zdsskaua.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nayxjrfy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2olkrkhqe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ommjkqhx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2neilfkxi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fzmmztmm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2djugxayv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dsvqbsxe.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uzdapnwb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2itzqbqhg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zbihwffy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mszuzjkh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gfulgsaz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cfwtundf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fbkeqamn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cygqowkg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfigxyon.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwquuenp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yobnilmo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bsrxbgrg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyunptpb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dadqtkzt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bmqjjaxl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzrsxybo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rwsnyjzs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xtomufeb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kbpivdnx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bayblxfj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2diuebtwb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lcmyxfvw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vgldlicg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2faibryvq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2alyfotac.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cvkwrcki.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wmcvkcvp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2abcirljv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zunovyek.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2solocprh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vtixaxjz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nzzugfbp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wspmfoab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jowyblth.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iufxqbmd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfjqunol.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvrbchxe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwrdwfa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2isavdndm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqacsdjg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tkmowodw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2etoavzbp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mkpmoqsq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yapynbpa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axjkllzi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpbcjzbq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ndokfned.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gsvbwzpc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wsikyvxn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zbeijkew.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvwaoaz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2isgqfdyz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zhbonqpn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hagworxx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zvgypmom.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2uydieuoy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wyjumzqa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jnubakti.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bwkagtnt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pucnqnfg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wcpeelzb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qwyxnmzt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2azbvhesx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rtzhkoen.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2burmqveh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fnydthwm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nbddbzfl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pbymejnl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gjxpazkm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2upwqradl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lkgacwyy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xvkuvkcx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wyoakvki.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sgtknata.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sknqdbrh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ssnwxedi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2zzvldeea.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ggbwcwux.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2keiagcfl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ucgbegxt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eljjpjnt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2clscepyg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2avlwiwhz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2dzeioldh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2erfyxwkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2juonezmr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nkkgluzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmijmiwm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2brfeuvzi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ypzvaupw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqoxaimo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mxzyoyzd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dqqqnurk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2kfrijdge.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mcrsaypn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2aebqnykw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmqxxiqb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rccdyvga.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zufyouop.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iaeorywr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpyxrigd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tllanlgn.html


<!-- 参考信息 -->