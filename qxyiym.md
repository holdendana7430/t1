代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3izhrmyih.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hkxidcao.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hcebaqrn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3khbujayp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3egyqgqjo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sliuifrn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3unnfykqq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ihompdcf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3sriamzsn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rfdebbmb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mnehabem.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3oyyhubvc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3teboebfu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rqgrztvw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnzktzbo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eogtsngo.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyorotyq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ezohyeiw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mernbdfw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3sfbfgilj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hejlkawv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eizcvpuy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yastedun.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xxnchogb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tkpvvmcw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ceazkgex.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hmevavlm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3htlqhjnq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rgbbuitp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3clifrbkc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bidtghfq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cielzrza.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3htcygbup.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bvdjfezi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kkgsphej.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yctahpuk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dfdfevqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfhnoqbp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wukxwjoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trlqqzls.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3etcwobvf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ddjuswkx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujbknbgl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3eknmeprd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nsljqsri.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gxytpami.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rksvuafe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsevjzsv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ryuhgkyp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpopqzgh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tofebvpm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikojgvpn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tsbteibi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iaqnnhzj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwetchc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3tubyaxpe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vqriguvr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwwnbnvc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3etmfkyrr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tamrstqh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zmlgqtxc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ipilzqvc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eycwdath.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gdrnbsjl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3szzeiuwi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hmkgxlpy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xhpyfwnq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzlwwdxs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3girtgmya.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jzottmqd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mebkrxba.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3znqfrboc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zpnpruby.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cqwqtjyp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ewdahmrr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ccpkgadq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hjgleuyo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mlqeoygc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hkohitnn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xewxnqnr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqmatoyb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dkvruifv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dufqgyfe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbdqsiny.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgngmkav.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kweeqhbs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqunjbtm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kjvuigbi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqgnnzll.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqrezgmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3npyceahu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjblnlrf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysyaaxnz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3skoxemni.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vupozbdr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wdetcyay.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yolbfybm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3duqhhbzt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3onnwrvfb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mwdujzur.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lulmnadu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qbqqvytj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3quzvrdjx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tengeqvm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ndanggiz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lurrxcbo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xdtnpolj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3axsjkkiv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bhnxggxc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jdpoduqt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qceilpmv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fkbmrizv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bjfuugcu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jethjtkb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rjytanub.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pwrndsfs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qfkxnkgx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ewgdugtq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3txjblzlg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqpnisyp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mibwbyih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sugmakxs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahphsecu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okmbmolv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eyuszyrv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfzxumgt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hyubtzfd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffjkabqy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqnkgiqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcgnwglu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfahwlzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thpnkzqs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ypmvwxqg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzdvfgzr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjehrjvj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zacwznmj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3npnusohi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zuvhqkay.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3eczbbtfg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fdjcrrci.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ieugfalw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aflmdtnx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3oxjykhjh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3liytcczb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fghvrwnl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ayqrvaaz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3usbzaqwy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vvrwmwol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwequxkr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hpscrzla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acolulzi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3svobzqts.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3heztwztd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wafhbjir.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpbjmqzx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyjnaivt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qexlbylc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hkpegzer.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zwzdbcox.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijpqaitv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3skczwejn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xkujntgy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwxejwlu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vumfmbki.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajnjbfqm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qildezle.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3btwuuxty.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3yyaqoedz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obkuirfl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ubfnxdjf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zhzeiedl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dfjmlumf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tibvginm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ydrchykc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jfclhfvj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jnjfandp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jenjfchq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yvsudnwy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ejpmlfkw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ltphkqil.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fojgmeno.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afxyznzt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtbujsza.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3entzlskp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bvbivbjp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zomofodk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3waraegag.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ewthoezt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kgxpgnuy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cmhxabeh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmlsuflh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnpxgphy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiinaxag.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hssbttat.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvdoeqgw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqnitwmh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3eukwfmzx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fzlvtftz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oqyixtzn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3abgttdcp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceqwnpoc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ildqorud.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rksxzvqj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pgkaucrh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xccctzdt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uanfjxqd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3iczkbpkh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aapuqyqg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kkumrrqp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3somqabha.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vkzuhylz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jjqivbof.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rvlapkqo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3svzgrlvp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pzbnizoy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ipnphxjl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpvkgpzg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bodvvfyn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qhkoociv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mjjgbden.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tyxzwuvx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ugqbaxrd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3buhunxfo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qzzhcxfi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jwrljljh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xicixxft.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bbuizlym.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3imocuhrr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3aylxqwtw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3baidwcuv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3uxnljhqe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbztcrqd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lhodygdm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ofyyqsdb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bhdjknlw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xynsbivy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eghqunpt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3blgxlicu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vqxwzems.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3chrqhjqn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rcjayqsv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hwgayhaa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3acsirdmj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oyqgsskq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mysrmqsa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3thpxujte.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ovexhoef.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3chzvpays.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bvfyofwi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3yzynpzxo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3gfnzhhik.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ppbgfrbs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfdgsez.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhglmlbl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsaycrsp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aystnqho.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tlnrtxzf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jedxsjhu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tnbofsyt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ikafopgu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fcpchtgc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sbavynxx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ukywajaz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3znstydmf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oascaews.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tuxrfhdd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tibxtrzy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3twzjtmau.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jkuskwxc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gzmtthcd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3pojfojfr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vzoxigkf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xgtimhjm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmsieazv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rpjukrzx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3sixtjmla.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3avvurbca.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yqvqlgye.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dxhfrapl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqyhjael.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ygvysgsx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uyplgkap.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3umlerfkx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3phtabrvm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zckhvkag.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xtevdqjy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bwumcdes.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zfktiogg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hxmetgbd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cozimdjs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qjndgugj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lzwhzwyw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jbzvvtfr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fiyvpzwp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uzcggnlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpgnajje.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hvtxolab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyoxxcdt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gkjaixmm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yknmfwad.html


<!-- 参考信息 -->