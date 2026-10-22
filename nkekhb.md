代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ctkcnxwu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bjjasklx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wysnyqjw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lxklsuoq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwemnoh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uvpyhuwc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnuffth.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fspkbucm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2yrwszeog.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kdyelqsw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wlnzsxpv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pvijblex.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjcdgevz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pqerlnhz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kmvkpufs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ckvxcdeb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zzfrsneq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lnvecvtf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qyxpxhul.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qyfkoaxa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rpvvqwcz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujsbfyki.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgbiodor.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2foqhismx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dxfcrhju.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fdwykhiy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecgunlhd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hudiemhz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rbsfwyoo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dpgvygzj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yvfnowey.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nrzaeapm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mxcazean.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gvrslbwi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qkkhbxwb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dkocouan.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xgiuavcw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bscrkeku.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ijqxshcr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2icaqfpxd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vncezkfm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2foafcmkg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mtnosfaq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2elsknbzx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2duaeblfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdvpxbmi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vlyirssf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnabihba.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xvxexcgc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2shjgcqmj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ltuybcsh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pxbozlvv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2isnwrbpb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2djmmxwco.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gqimifks.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tstgemxq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dlsekxru.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qcdfregb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rdekhivd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttgladlp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqgylwls.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kndweqxb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dgiaxmyo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2abmiypeh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wixtdtwx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2euioliwy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hrynzbul.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pfbsgtpw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sxpimill.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gvimbrcn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2npzmaraf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bwglnuae.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ddmytter.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xphrndbq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2agxskfno.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktxdfsyk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qlvijnqs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ysuzalwv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xtvxzaur.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2plkluial.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvzsmyr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yrbfthsm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqftvlle.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mblfbjbx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yoeizylu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2thosbohr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2noivcmgi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbwggghk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qsfppiys.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyfclgyy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfbgrrb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwtpoilr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlmoydxj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wnqtdtzz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smdpndtv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cbghoakn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhsqldal.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewbaudwh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ibmaawwo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atzvwfxt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytqgsjwv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzijooby.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tqhppxal.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rchvopge.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tyhkwkap.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eprsytiq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wbepugdp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzhqjgle.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pgjrpwxj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mhzklump.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wmemghgf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bmbygbnh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2uszoutft.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2achcfkme.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wzuhqtoo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nfkozthf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhqfqsw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tlmyljol.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kdpmthbk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2atrlddpy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ualmzruv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pophsdnx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzvldwog.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tctnlepj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bhluznob.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2msprmtzm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2epmfzwgd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydtzuznm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bklosmmu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cpldeefm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcobucg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygrazvve.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pneepcvt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2knizouuu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jkgnmskk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpldyzmy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipilcvhw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkvjkwdy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vglriasx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chqcqkut.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ajtoqezf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxwjqeog.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhfbcoiv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pydkpufz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kpzqylvj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aobozito.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jihfjxqf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pjujobal.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mlbaydsl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vfhuuiin.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gtwcahrl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gehbhgqe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hbmngsdn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ztzxhohe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2byzwvdxg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ghakposc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opadinyn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tesbsnjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkzsdrwg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2shlfxdbp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yrogulkb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pfjgxwal.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dstwklro.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cedhbtft.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ibztrflp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2glujsoec.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wxwfhauo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hrcoqqdp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shkrshtl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rcthrpzh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaybvqpx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsuobrdp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jndqyvle.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qmpeddtm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kpafvikg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kcwvcnqj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgldaelc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xklodpzt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qtzcgzyl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xxveioni.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ppefxksb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ybhwweax.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qrnxfmjt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uvrambpj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zkroiqki.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wtwxtdim.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ivyoxykm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2asjdiphk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2znwfpkll.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nvomijgc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ipreetkr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjplpsrn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wrfobspt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jqtvnlim.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cfeqcdxq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2brwxniwe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rcloqugc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cigeepfz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdfohbfe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2blggqtnh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvzrkgvr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jqhfajoq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bzzpudtg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dubodymd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qwoybfzg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zfkobwwc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqwjuibl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvhqsxbm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqjklabb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2molqynho.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zpcvokla.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncxyoidv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zcufsbiy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xnmoldlw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wsslkabh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2btkerunj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lowzweck.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fgmuhdos.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2faqwaxqf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vlfoefcu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2oyqiwbku.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rcglgfkm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dnkydnxx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2aqcbjeeh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ruirnofk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrlfbhwl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfmngqwv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcqvusxm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wkhmsvse.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2blacjkud.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xvivtfwg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nfwmpfxf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mkapvjzz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dswdwuim.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qqpmbuuz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzljmlsz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lcxojygo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2uasfsqdk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfecuxsh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bjjgcocw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jtbyfbvm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xqzbclyw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dbdjgwva.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sgkaeedl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ekuwufvn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vmartucp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2seqhyubi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tzvdiqcg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2llgrhnvc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rcxgvqfr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mccmbtup.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhugdbum.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2leszptzv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffnrlxca.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2roccjcew.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qskcmcou.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wfucnvxz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dzvqling.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vlpaohzg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bikesson.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pmrfohvo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vbkavdwx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmshmxtr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aitgvmdn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yrxtolwd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2waxcfmlu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ptietemc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hhwqzhdt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2eickgird.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qsfbnkdo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ewzhwtdy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nhxseayt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rqlmenvr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fdfouiff.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tudnyvtv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2durhrniq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fegydbvy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hqsljmkk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mtofmyaq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gelycefg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dlfujgcb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hjwqikyf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mdwpbyhd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jexgwevy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2abitgaby.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2urnvyjge.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2icomhmnx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpogwicq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xpwsnmmc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rowshngt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ijrlclpu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mstjzaey.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jvqomreu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfppllfl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ussoclol.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hqyipdfg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gtuqnupc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cbhopulu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tkrgjmjd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2galpyopm.html


<!-- 参考信息 -->