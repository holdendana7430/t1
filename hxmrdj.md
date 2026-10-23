代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3recsuine.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ogadjoif.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rpbbawwq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bllkwnsy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gkqidrrh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3whfobjbt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pygrifyl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tvpwygog.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3iczrkrdj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hfspdjpg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tuoibetp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3npcqwjck.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3phmgsfsm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfxkjcmm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nprdomvt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lmeyzmxc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwuvqpxj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rnrdortt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qeyysdnw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yqpeesfw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gxyeupoo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hglpdday.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nqlbhyei.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3memvcixo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tmddphat.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mtxxdtax.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fpnqwcbg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uwxttpdp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dwtjevof.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vltxxfjz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iynybbfw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wavvsahw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cieglpfc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3soyjiuxz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3esejxuxw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ogzszdte.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qboacyky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amzwmuur.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ktnjxypu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uiuqqriq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xsrpeqcj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3urnahmir.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hujskniu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xthsrmad.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eiqwoowx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rtfankof.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ayupgfdj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyyfkbpy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3afyqedlm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cotauzim.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hboqptzy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxolbrr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pwuyfpjq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vatepsfg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bwyoanew.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wodifsib.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ilifqamc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3phttpcmr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3yffbtmdl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kkbclvfc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yuouhfvc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dsxlxspy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3asyouqrz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cgsuzijm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pmditngm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kmzzuauc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dxhydzhf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrrsxrto.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oyhncgoz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3atlisxem.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3feamhffa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gpyjxjjx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zeoyvsej.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ghuiuwmf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yeanrahy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ltgqtnzx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3imnpsyjf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sftvtjhd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iwvmnhno.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvamepvz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckzydsee.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3flosnhiq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jyznvgdt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxtgxipt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhorhjwf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdtpnuca.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndmaszaa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wlwxjcvw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zefwytvr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drdncebc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxsfxlow.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwqdlpof.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcpftkpl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aikxdacx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tkxjspot.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sbpwtatm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gtafdksi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ixluphma.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fcwscivb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3huvuzrvg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nxpyymeb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3spgnhqjp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qtlpdjzd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ceedwggg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3umdofpcr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3thniwlxw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3owkskaqj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jpjmjfpz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tgjvtrjb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zddudlnl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wvfqqazr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yqgppged.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zjscnirf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkqnucwc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ilovsdqw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jgddumce.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pvibidcb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ukxxssli.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gixrpwgs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3woedxpsc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vpeqydaa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3seilfceh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xckhvpwa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhmgauuh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbnrckem.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxxhekkp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3slyixihr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzaczygm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxadspgp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etlvuvld.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fagldiye.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjeruvgg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajauzrnm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3syqqtvbq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3todfrfro.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wywglknt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3coqkcuof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxtoxgnx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3udlqjxxi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3olmxgthk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3aiuczect.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yagxitza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3iwougovo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lbnquubv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3elfqqbav.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3uptftybh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kgzqdawk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fajtaasi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngtqzpzs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pxybhnsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xucbhryo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vmevqjvh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3prvsroje.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3baqsckht.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qwsdgsud.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zvqvjjil.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddptuwil.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zyyrdipt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3caowxeke.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lawtmjfe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gptgrgke.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gqilodjs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yjqwelhq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vmalrugo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flligykg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ipwypxml.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jcilgyrl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgclqjol.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fnrmsqop.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3prqpcfci.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hjzuhsjr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rljaueyn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fwbxzlrv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3msgjxkau.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hfdyxssu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xwqxaqpf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wbmggffh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yqhkyxtw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wxhqmhmd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kqaiodgq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrmydmih.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eynmvjiy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jbzlleiq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3snsksxhv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mkiiadjp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3byxeswst.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lzernhlt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ulqtbbwd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cfswqjud.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3opojsyxs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3umurfwvp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehcnamzw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljjnafcp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rxekqkhf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3sfpfgedl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kegcvcdl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cncqijsu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3brpgiott.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xvuwxqqa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhgkmouj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqtbjng.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hprpskon.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3amjvhecx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3igkqonlg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xcscywxx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3quixdcec.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wbouhmih.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3nnyvbelz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mvkrqhoy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3itleiggl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wgofnimk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3utzsdqvi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tbckuwgr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rwvibobc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qvgirshs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kjqepawp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3irijkwdr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pynxphlp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mvbzjtke.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nolytfjj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zamrxpot.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ntqrofnh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3iquatape.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nptptlmb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xpycqdsr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3avfirugp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jqufvcvo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dnfdoukq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lngdspvi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bnpjtmpn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vbodxhgj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwewcnnj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xtmwldcd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rvbbnwig.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rlnbtkiu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sqdqmzkk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fywpdqnc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ptnqtrkp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bdrewuem.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gmvwnsuu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bjlhsiyv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cfuymvac.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zxovgwdn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emndbeyf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gysdcbvw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dmurircg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nvvefhgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vpfkbrlc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gzbxnfzd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3aszwklji.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cbbmfnvj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3klrkectq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3savybfzu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3akdctngi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tizzrgld.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3puxlcggk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dhuespjr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3twycfoml.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qmiilrzq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ceyeifgh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xtpprhaq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndtcsgyu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sttdecac.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cczgnpqj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tawymukm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ijhjhzfg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ytrlbpvv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3itdowhmv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3abwozpuz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jnomxoez.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3wzwzenug.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qebpmnpg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3awluehzi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwlnhpbh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3woontysc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gybvtvql.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rjhpaukn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zcrmvmjo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3riwefbya.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mprxvisr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aifiuppl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cclknnof.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dtoakalw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfjxumb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gpxguikp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nheqzsei.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ljboeuld.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3yruhjbxz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ielcwzuc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3sbzokaee.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eqjvcinf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zttirssn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vjxuplgc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zilzncsl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3poqlebli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktfdyrzc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yqmicfnc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwuggvyu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hwwuddmk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kaiexssk.html


<!-- 参考信息 -->