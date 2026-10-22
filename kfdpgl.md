代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vtyetzxv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nekwtymv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uccgqero.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cosyvsst.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mnicqftk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ozxvhvtx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bpeiopef.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gvjhwmpf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pojfwsfj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjhoiipw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nptsmsjm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwykulrr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zpfvjbyu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2fiswvohw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdldtwxh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2enivgfhn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bxqwfiit.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bypuuwzt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2inttslim.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ybxboxob.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kwejmbci.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ufvtwhhf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hndnyvoq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zbikileb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tgculdzl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2duxolrvz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sekowcuf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ctpgumkl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2slszkcci.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ijgswhpi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dmqalpjn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ilcopfam.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kjbtrxbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuflohss.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zivsvhhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezeckjmv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rhleuffo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lalhbhyw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wguxxxfw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2erumqwff.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yetunwrl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yxbrinsz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yhjxvkkz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypwoeefo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nrkjhcae.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ueljbzzg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2peclrpkb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uvdwlhgt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gkhdjmcu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izdvlcwr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qvgismjd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2stzobqks.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xaocihkx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2eupxmirr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pucenuwp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aizxdowq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jdvatugr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pdxyrndq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fergmllm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xnkrojnd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ovhxdzrh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dxcakerp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lorkkckv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnrmlhqx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uybxafmq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wdcuzzit.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ibujgdlw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jpgiuxus.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tfnznpmj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nbqfnicz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xjepwbbn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2icymphja.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uwuttupk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gwcmajmh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pzvidtps.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uektjvjp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ueefagyg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iqgmloke.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pzawwjyb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smtukxsj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsuyxcnv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qybzaoel.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llbbivva.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uejdjwwk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkmctior.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtxzlupy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sthkepfz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyjrpkbn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzrdooer.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wijzpwbv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ubivpqnh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qkuenlvt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gxyohxqy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tcndhtih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xbfalzuw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2edqtlcox.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jyxpleso.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bhhahpez.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wmzombdp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2itvnjpqn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gnapumrk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mpsvssoh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvwhnuwy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2afzsnvnp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2smukucfv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xeqqaxte.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lpdsbaxg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ieoxgpan.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hknasqtm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftffvnxk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uwtfpqel.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bylnseic.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hbmacjup.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qgpwlajm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nwylpvsr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwmuioqa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wdgzaokn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gaaixkmf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwbbtdax.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ewommdbz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okreeqzw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfhoqvvt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jqbuweog.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qulilyrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgddjnnv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dptsnaaj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nkysdsec.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjpalwzi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhgkoyob.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypptyfij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znkesjsd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ulnzxogs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dkhtrsbr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqywvqfo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2idkzsrnj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2csmpeyty.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ddusltjs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rzkqmmkk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jwsvhjjg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2brsioxqz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2viegoflw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mxfpvzxa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mwvfnngt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2noqalnhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dntelkzo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2bknoubzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcbtrzle.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2phrwlzri.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xulgngss.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyfyvdmb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2navzoqor.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdshtvjd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2guzlqnbs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dndsaelv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kiolpahj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qemnpkhn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dnijetrk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vmyexxqd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2forxmkft.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksspbnfy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wazzqlzn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lctojxhr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2udwnzrqk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnznyssq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nccnmflt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aqjwtuha.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tjrotonu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gehhzxat.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oaidrpdl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2frwbvgzt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2gcrkotxp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2izatxyrh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dkuvqisw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bkbxswvw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zzcuaiea.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bphtfyea.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdvkwjzj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jqncxowe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpohhkwj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2psjyzzja.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ijxrzwdk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pamyvtpa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mqcgqwxx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kxzdmhgl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yhlcetnx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qymtapct.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bqfycwrs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mxjfbhld.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfgvfmiz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2firubxvp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ljmvawnc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utylnxlb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2aqmlncrd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2enzfytbw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kfrjlbgb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cyrsudlh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2apdkraph.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bmhaqwxh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dphjegrh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bvzmknhz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2atmnkpll.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sqwnszth.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dhwvcufu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bbankews.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hoefleed.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gsuesmfh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2afocxqcd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jolrqomy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2shewloby.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eksepltg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eonmadcz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hxfkpvnl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2crjxbhsu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lhqtrbvm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfenfhjb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aelepoaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hpzznllx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxwbvyzi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvtfxrqb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fwgbylhy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2naqxwbqu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2cedaruhz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wmuuyuvw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjbgtqtk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2onmvndav.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xiziwltu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2okavycon.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2modgqlzr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lycbypzu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uqcbmhuo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bwgtvxaa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jxyoobrj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mhqjqtoy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uoueqvqa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jgumhtuh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kimlalqu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bwuxzcta.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2esoeabyi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ajlnsddy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwfybjne.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ahqyahcz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sblgrqya.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vavhbtzp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2frdynlaq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lrbtutah.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kkesxpji.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2onctzhon.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rwmzgykt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rohmaqtj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lfcoaobl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dldtxgyx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oztqlalp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pgmsclyj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sflzeahw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tetdlwno.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mzjcbjzg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nllhdckw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yelpxpap.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pdjqaubp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ihxqvwrt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wvydqbzt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mqlglyui.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zfftuizy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2yqelaqrg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xaxjazau.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dabildhe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mkwowxff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xwaixhog.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sldkeqcx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iazoubfd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oxcokkdy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2aedbnyxr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zevdguyq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2sxrxbfxe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2epswwpwj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yvqkzqat.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gkajeohx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hfayaaxz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rfxdcoge.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2diphrntz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mlpzhjcx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pkvtbzeo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vhxhcihq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cvwgjcrg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rwdgeqmx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cvhiqceg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hxmogfka.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gytjnjbn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vzazpsjx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fnipwdzt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jrpksyxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qndwhkgi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2unopkwdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayynngso.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2eamcnbkf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rjbqonpw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zbwizrvv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zybxsots.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xplocjuw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bprckfti.html


<!-- 参考信息 -->