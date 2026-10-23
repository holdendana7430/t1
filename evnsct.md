代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rruihjus.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnnymbpy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmqmjmqa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbrxbhqt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xmrijkwe.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3stbcjofk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcarwtxu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lkyakcwu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rrrrkyng.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lgldvnps.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bbqsibjv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3toiduuma.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zlcfvjqj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nkqsplce.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uvuofewv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vwiqdrpm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dukgdyyl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hpqlqvnq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ydtofchh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pbrntgfw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxjbsobx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3urcghyei.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kurqrxqv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tqqwhysh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ykktoulq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhykzpad.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uyldmgaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svilnqum.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iazqroeh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qhunlasf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uywgnxia.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xgvuavgg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wajtnmil.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3amzdoipy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gbayeixf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rvfdninc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pxqsfcyv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwkyydug.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hydxbbln.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3slpfpsvd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elwiqkch.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pseiagem.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wsadsipv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tgzrszvs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rldfckrt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3edetavod.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vjmkiyqm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nvvyvbno.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qltxtfzw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3svdxuzkn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mggshxga.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hfuqdfwo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3lbopvwpg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ywibkheh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ujtttqsn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3elbgnkqw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mnbhebdz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3tfeloxnj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rjcbnvjg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3czpgwpjb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xiwnfwti.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3alxydxit.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zsqqhwlr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fdwfoxzh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ozfjmocd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zrifzwel.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3niulfiad.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zoygjiqs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uphxbjos.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xfzemdbc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wjmnprgx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpqqntsa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkzuwsfp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3eyzoojul.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnuioxpx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3shvzwrcq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pegaabzj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aarnwfev.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uabpesfk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3getniosk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xccghkct.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3efwbhchr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cogygfkc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ejyknwtt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jzvijzfe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3khdbaeny.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pnahvwrt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3inqebizg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cqylwivd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ivwlzrij.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wxoooles.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yhxjofvx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bhrlhpye.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rtervhah.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fzjiskiw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rhqjcxqe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qcbrfkde.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3tnqmvvlg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rhmjcqir.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zkoogoej.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zchlyrxz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jyadsvzi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vkhnhcud.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fbybfatt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kjprhkky.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pwjtpkog.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pvixmuek.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvureeky.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3znxvbkyr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3phbroych.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfjstdbe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwbyiyle.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzeabdia.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nybvssqe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pclbcigp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmkfazbn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcsbkzoi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sirwowkc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ticaoall.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3viahphdp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jqeggjdc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xskasjpj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umetkqnn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ptmznzon.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3maxyxjau.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3phbbmilp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lmilborz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3aoffizon.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3cqueoxoq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3adgzgiws.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jwtnkbus.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gsioafma.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3fpsmrnoc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ccipdxsq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vjqiwgcu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3udzhfibm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xuzgibmj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kbowitto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhaczemn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uivwzxxu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gadmfasb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kudhcjdj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3evthueqz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jamrqglx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qsajkzzu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ksxtzrnu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ysnfaxdz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3smghroit.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmmzuwvh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ccgtymec.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qsjmljof.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfvaljuh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gandaota.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tjrkstch.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yhykneej.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3csmentqd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kexvbizm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vxzggdyt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ktpvtjkd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3knitzoaq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aysonmjc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ylzqsoad.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ezsiwijq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mesakrdm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nvyzvgxz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yiigytjm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3khpufflz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3doqdnkns.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fsfjanhe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ymvkerzp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odxbtrsx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ozgkvzky.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3guqetnma.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvnylfix.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fejgwllk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3blvrpazw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cjtlrqjw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qshdfqgh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kwoacfej.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3axiaakts.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aeboqece.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uonbbblo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cnxxdeno.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3smhgnkjc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gmnqchqv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3syzqlbmx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3msdhwywg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jdpzyjot.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfakppbs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hxzmsdth.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cjafcvuo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3poulczsa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lilxteym.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bybgpepz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3zipfjirz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3upgqveht.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tflvwhvs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3phctgiew.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hjqegsdt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tgxoqmte.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3anlannwh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3racafnvz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wwblyoux.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hycnuwwu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3slvyxanx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3euhwswzm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wcsflobx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ijhovexo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rqpvgibj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wjjfvyqq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3doryueiw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hagxiiwe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mppgkvsc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryhhvwlw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3klumsrvv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzempnjm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rakkltff.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ttjybzqz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3icggezvj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dozkmqga.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qttumryu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3abzsazmh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bbstxbhd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mkrsxdhi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rbbxzaio.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3eejyxaev.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3cfyyiuym.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yoododlr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zlfpupms.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xtcrduig.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3hpatczxn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qobcuvwy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3woxfazpy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3loyxrezx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ppemcrum.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fkhliuud.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lxuunoau.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3djrcdifh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fsckpoat.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uxhdbhrh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjwzacjw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3moyojsyr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dfkuvbpg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ixzvphux.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qtqbqxpi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bmvwtbsb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vhldohvv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ccwgtcpy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ptpauuqf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3avtvjscq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zxzlspxk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gxhssnsm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pkfjacxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dyaovgoa.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nnppvamk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3evqlklqd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bvzoensv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vztfehqr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fvbgydyc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3igumafvh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dntbmwav.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zjmaskwr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ugcfomaz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rztjmtxc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3uobldyrs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3emnqskxp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cypovzdn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aefctvnp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3npyzntqi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tshpwcbn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jcbictdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwedawu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3spkcljay.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3asjvsulr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gcqchjmw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rzwarpoc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zffsworp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qsnjdsed.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhysefev.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jaxehasz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3evqqlaqg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3nclywisw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ngwjqipk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpiqgqjw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3qjmdorig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3itufcfnr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zqiheyyk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nxstwhqj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kelxwono.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmoqthu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkofgrja.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3erphruwg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tlnepgtw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujcxqmlt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dronkfxe.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gatwzyal.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qtobcsod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3quiyyoev.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3toqdagom.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxfyjdya.html


<!-- 参考信息 -->