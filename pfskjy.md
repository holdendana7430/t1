代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bhnnzcjs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ftycxgoo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pymodscz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hdzxngun.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwtqglf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lkpmdpss.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lgbdxlhp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tmnugujs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2tjtvwrxd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pfpctlkh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vjipuoch.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2flfwzwzr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fqplyrly.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lxguvscr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mduhprdm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiiihcyb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xyuyturv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fqvufzfw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2coxykpex.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uwexdsma.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vjfkibqe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dgwdnvbl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sohktstd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2auoafovr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cibzyngw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ipjkdgnc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2trorqpgl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dkdrpusk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rhjngxic.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cdfgbkrv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vgiajdbq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kbiojxwz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qkjhyydq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mexxbcvc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vtimgyai.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ujwfslng.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pfopjezj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlewuelk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2nawgxtob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujxsdtcf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mqxrjozz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tlsswcwi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tzldgkwz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oygzwbfa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gycisuho.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2upjcezbi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fwnaegbx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqsfntwk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kkdcaldh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hpmwkdzn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uwujaqqc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2npjvqwps.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kqasabbn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2urqfubes.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dtirjhyh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jxnqzrru.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2twywrkjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wjzybmnc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uzsikztv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ogxulznd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yuxegujt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pfahvyfu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2byntcyhx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ywojxphm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hhttzatz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bkhefeop.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gqeoxzam.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xrqrkjlc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mtzdjayj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2twjrgtzk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ayxiborr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xxjtotym.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rjvfemyj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2agbptwyo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2twvicbfw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zurqqtjm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2olybwuyh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fimqfwfw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jwarrodj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlpvvimp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwbdbswa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pksaduji.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fjvbfcob.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2glwwugeu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bztyxtkw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hxxixtyg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hyqntzeu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2japjzexw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llnxrthw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjcygtda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2reqqnhrj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojpgsfxk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znbcruql.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wnuskrho.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2fyckltch.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gjobrrht.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2paplmupt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wthhennx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2exmehaao.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qdwdyybf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ocfapmtr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hzbeafem.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vhphvvvw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mqbnukle.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2azamaztz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2aidtukhy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qidzgrhz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ygcjvkun.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xdxoisai.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jhedccme.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wjrwrqto.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zqqgzdey.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ygpkhmyy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gotuouei.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2onmhbvah.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xpekmxmx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rviyephs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lyvxyzzv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nkernvsu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofysxrmc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uvlgwkcv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2owlcmarf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbjwxjdx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2toitzknb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfhfmjba.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnvuitgs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2optzdcnz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhzehytu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etifzoof.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpvrhhkm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxcswjrg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yyxkrypy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2aiybhrxa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sexejwwh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jclxemud.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmxmoxs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dygwvvmq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upshvhch.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sdvcspun.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uepopfrb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2utsqdblf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fdmznzhy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2myepccqh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2znhjzjmv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sbssdadz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ctddpkxc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2uvyosnqx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zqcugvyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kitrrqsz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zrgkmsrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oadcsjpz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ypfrvujz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nzqqbube.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxudleaw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lomoocec.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2siywjjvh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsbbysmr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2amcaoofj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2owniwkqn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqdwocqq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rlkkmzex.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fdqibbid.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vbjlhscq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyrovrrd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2muilbvqi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iwiphonn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2thmwkssn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rheawbal.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgjirzjy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hgnnhlvq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tenhkwlj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bgquruxk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2byzbgzcs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cabjznpe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nrdanjzw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xloviksy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sfpsmekt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lzcmblwg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2katwiqan.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lftpokhk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ducqhwct.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sikqscey.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ovmswulh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkdpngba.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2clvhfigx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2twdvtmve.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wotkqbiw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2awihmxrc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2prnlzijc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovabdhlg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jytkhivk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vinopiym.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttjjaxnk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ijpvzofs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xgxgsbtt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kglhnyua.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lgxmzszm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kqwdaxbg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rohzmdxa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cmvvjyjl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wmzxpwwu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2davdwzgf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ovbavohv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2butziary.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zohsemle.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2awqzdukh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hrdwktwi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fuknsdgk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xnfpepfl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oxgefpqq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ivnyczig.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kygpxxnd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hllktuji.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hojyvfaq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2egfcbeoe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lkghxebw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvhrhnlb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxzszspd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cnbmkzdk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2umjxpgav.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nluhmuzp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cochfzgy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hjtxfoaw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pyrsnigv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xtmpetkt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nntqrvnf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gzlmsumi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjkpysue.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbknmtwl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xzfwgpls.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wanurjdq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2drzpytmh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gzybglvs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vvobfghh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yzcleecz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2txrcdiqw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jpdryuht.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2diktminx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xfocatml.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ohzvxtcx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rtubxjat.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2razzqybq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jcwfutke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kyjxnvvv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mhfkoqir.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xprzaigf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ytvpmmpw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2agbpkimb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fqhejzjm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qksljths.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ulueghhe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2urhcggaz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lggxhado.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okjcrkyd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmdtgoot.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sunmilrg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2szbjhgfe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vpvlutdi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wlrlldtn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cdqwzkfg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vljafuuf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hnviptda.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qjemfsyp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tliautnn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jzwfvgbx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hfjolfsg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfghmpl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2damonrdp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ddyabxdf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gcqovjkj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fsqimknm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rzlxougp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bktpsxck.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pbvlmein.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rdnefpmr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gtkvslau.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xqckiawi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cudlrghe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nslectpe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycmesdwx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mumdeqpj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2evcksxke.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2moslzivk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dlfvndfm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pqybslpx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndffjqwi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hcosacfr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wwgaancx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cpcjjmpc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2znmlxttl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oiulvkix.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bfgkvony.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2evzcpzqd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tcyihwjh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tqceguwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gldnfrkw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nqbdjogd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnakaovd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2losvuwmv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhoeynn.html


<!-- 参考信息 -->