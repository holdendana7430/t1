代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rgrwivyh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3txpppfhu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yrvgykfb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mwlggngk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wguhkoxo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xlnzboab.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3oucnmkbu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mmnamxli.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vticdrbb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gndcervy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hcpytbku.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3thbsdfaa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wpyuykso.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yfyctqxt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hipgwatx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fblnnace.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ggssmwdj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jtqrioni.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqqiaqec.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ulgfuinh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgqpspeb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dsabfrvt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3twzbhbrl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3epxbtrwu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qsncdrmd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xghwagye.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3paavqlhe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3osulrlrw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kgxqochf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3iuigtxce.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pwjfgpex.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rymunsvl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mtowzihl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtbhqgwu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ocbgipun.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rmajajux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bgmzvzzd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3asbnlkll.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sgrckpyu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iojhgrjz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qjwjzkta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oixzapsn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jfenvycc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlpmkvuw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cujrlqjw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3coghdhxz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wwmfvhfv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jtfxufir.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3epswczqz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xxrkkgdj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hyayqvlv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zchjfigv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jwnrtlbk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3krylhnpe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ykxqfeqp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3axwxysjf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmdfnuik.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvwirkjk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yzvwgfkc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gytfrbeh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jfaxmokt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cfdwdfre.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bmrswsgl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yriyjlsu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3onisfrod.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bpwpivyy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uqljcvzu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wgddlylj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3btzhifgz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hpedfbxx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wibrkedt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mhylzbji.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wwqvxvgq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ltklzyhf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sjcwoxif.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ljuelaqy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3pgttwujh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sggefkau.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3okvvfvor.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uglakeul.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nixxuibu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yxfjsskt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mzgnhsww.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nufziovq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivnzmjuq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3inlpnuzi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vpynyhad.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mesyozea.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hivwydup.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dldvvduv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pklpcoaq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qttkijrb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ucctsxvm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mifxrpuo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kgozmnce.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtloqiug.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ynpmpqjy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3voawbvdr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3soducllh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bncituza.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mzqbauek.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3abjyqofv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vttalnld.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dmyfzlxq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3opcthjrm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xytohtcv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3baorcfgk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3njpezblr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xxgyfwwf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3oejzuylm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hgahitzl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uqkxydkw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfjvtgd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghswdqti.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vnebhgwb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uszvljvc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kjxclfwz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qaogaykp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lozxblzh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dvthxllf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mbawlwrp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3szalittq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jnnusmbh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrzwsnuz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cxejnlrm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jzyjhrhg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brlbnlim.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzkxrnxs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdfpacvs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuecetht.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vrbezmgm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjcayixr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adxigyjz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twlxvbck.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3izyhhnut.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmbfpepa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hbvyqwgb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eluvsxap.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwavdvnp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lxyjieic.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fyaeftgu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iapjryez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kmzdpwpk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ezjwlqix.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hsdttomd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3sxvnvqrc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3shmzeuam.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dzetlvvd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bfiwmvdz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3frqtuovn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3fdcdwtql.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sejddtlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqncojal.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qaqdukno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svpnxdba.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3edtsfmws.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ckvogjvr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3digfcjdr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcvtqdfc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dcenaoei.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vztpffmx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bequgsyj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hdgwtdtc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqopjkcs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zoruvmnj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nvcbixbr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ghylrhcd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvobmrhl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3azxevjnd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3adbqwvdr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pyvwsiae.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttdapqyd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggtfpquq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pvlyllfg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ejnudhez.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bjipmphs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jtaytrdx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yndebldw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wwsqkddu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nufamwjw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ckjtualb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3attvpobl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ljdcblac.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3evapxwdm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wwoenusy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3exhgrgvp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtipkmul.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gifftzdg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tbukwcqs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zifyfvbk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xnrculhk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wsdoovpb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tmvafcol.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pwpkpmaj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3omornsvz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgeevvzp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tqfuamgx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ymbnlvga.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ichlsvrm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ymghjbyf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wscywuuz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3yieumjwu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3smrrowhu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnuobwrj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lawzuism.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gkkpnszp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gsnddkwr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rxgjqrsj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gyqtqmxj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lhfbjewq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hpafjzzq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oqappduz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lnxwlosi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jbbrhxjy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3prgritis.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mbrbuzsn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uqawnnss.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bjpqnltx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qsdrktuz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xzuiaadd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3liogjtgs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3amxiehbh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3msgxrfcd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dhhsatdu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3munoeppi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ufiwevse.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxfjwacs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kqqqixmd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ibyfkchb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdvpdtdf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zcqwqiro.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pdeaswge.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjtxfwig.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yymqrrjq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gpeuryii.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fntqbwmk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kumdugmu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uqclehga.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uizpnmgz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aqgjicnt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ggaybzuw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yiofnzqs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xrjzenof.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qclgvlcc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3seqfruot.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3otcptfgw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cauwddma.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cccnxkur.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3stdfixsz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cjzircxh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iosbiatn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lijifbco.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3olicpymd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dzewuuja.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mjmnwyhw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vbyeyiyn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhsslqie.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3klohogzo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vucrzzos.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpejtpss.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vwtqmxos.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bwkosima.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vvmqqchi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mdvfdkrm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cfyhggtx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3shyblaal.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ycpexxob.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pukpujtp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bnnuqfki.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3bfmbbddv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zgetelic.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3edvcopep.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hmnifrup.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vlxmcvbv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3alcrahto.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3chubrmcv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wqflyzds.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cqalnkau.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gnxsptnx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lglpwpsm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wqoefxos.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3njwzrvke.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hrdakzlh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwjunaba.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kyufarhp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzhaimt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3axtgemlu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vbdyiozl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gjdhonip.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rnvzueqh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lwhtclls.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wwddvbwq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wisybmyl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hmglzetw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqojmst.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vnitedbb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mqxpwdrb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3frorbaqk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3juqlzghl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wydwswqw.html


<!-- 参考信息 -->