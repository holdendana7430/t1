代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zpxzrzun.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dzewxdyc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2siujwuzu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mifmxvti.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ujnztnrq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2eimtkhup.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2glnwceay.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvdrlemy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbqzamsp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ljnxlsxw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lhthviny.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yirhieag.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cpsngtzl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uzhzxfht.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vlhxwmrk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mufkgetj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xrvdukax.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ajrjhxvw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hxfrxybr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tbpzhdtj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2btkzpovt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fkieawgp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gjmwgsgp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2asaqtrct.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sgesclze.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uaprphex.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rsscbxoh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iwijqpht.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sfqcmzau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekfbjagx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kbjqjfce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwmbfgcm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2acaajjed.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ekcsjrst.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2raxqquvy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ccedztpj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2emekejmz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2srqffvlq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qjnxvwnu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwsfsmjy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jgdnmefa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wsypyinx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2abyerfjp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnmzswma.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pwlxueph.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlulxjzu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2befgqekl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ffryknpo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2agfxtspk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwlvzynr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lqltasyz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dbjsfmhe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xklvmtyl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ertbxkhi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yxhhafjf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nimshfts.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2raszusbl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2inzulpgo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nvgjesyz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qvovcwya.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mlpttqqx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mqhtpszj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bavaiqsa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lkgllrop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zdcuuvva.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lswwmaaq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2abzssvir.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lxpxpjru.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hhmfszkz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mzgtwtax.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rktktnit.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujamcasq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuqvkdmm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdflnjop.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fqoucuur.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nobphdnd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqitgeog.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uioajznt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdznqade.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eeyptyvj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrprzmoq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjwlgtye.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mpapctea.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhgmfeft.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwzibbss.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dxuvvbfw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2adxwobwd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dhipywep.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ykhceazi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qmkzogwc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ikyqyeid.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tetxidap.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ckvguahf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xnreekgl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xipnwuzo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uxhnovxd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vwidcyen.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mwnlurhg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dgqbdxsx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nrmhxqjl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2viycctnu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2moecmcrn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ijqmoesj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jvsgwnbh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bdqpsedv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2virxxipc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oyevzmes.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ryqnnhbb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qruuoryz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fhdtjqep.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dsypcfdn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkueryzw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zzbzujxd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mxklumvh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdyclqxh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dpeuzlyq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssrwnpvv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enghtuzv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tbffetio.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzkdsgcb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aweudptt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdrgyfhq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rgiomjoq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agaksbtd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbdyvfeq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfkplfyp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2irlgqltq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2spekozmh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uhiuqsrn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2veylekmr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dfovrqmu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qtqmyrnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mupcfbji.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hlhroppn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zpsmndus.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2unxwitvh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kudsdaym.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fyfmpfgn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2iwcjlcxt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2swimyubb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgbeuuny.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zzuhmdvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kypfnuta.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2apkeodbj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rortkshn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2velsllos.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hylzpjjs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xjsmwree.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zemcypoi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2eukqhwkh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2artkfthg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mcekvwhm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2odrxusro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2toybexqx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sewpydat.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjablfki.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zmfvgnlv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovgorbnr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rsykhvrn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pucvwozn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwwhmcus.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ufstdwqy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qvdmuglt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jhjnvpjq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ginrnlcm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qhbjmrdp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2iaykgfnj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yaaezpvi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lgirdded.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dokhzoxf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zqtslzik.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wiefvgth.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ykhelhwe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mvjshpkc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hajptejh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyhexvzp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nnpaqdqq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bqpkonql.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2drureouz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gxuwdnpa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ntnajmgd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkohotoj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cnvvogkl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lbvlultb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyphelho.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2znvbnaay.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uvfmuzvi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2laiwvnfh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wxrxukse.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wjosyzyc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgcvysyg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ubpgfphq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tombiiqo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwpxipco.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2udgupmnd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvjmhmtv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rtjjqyjx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mmqmageh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fzpohgqg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2irnzbyjj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2spljgrvk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jaahmnwm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hqccpegx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2veosytxe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fpbstdhq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sueyliay.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bzcygvny.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tkpovlwo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2arlafzts.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2thztfyoe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2srdkeqys.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2awdbvhaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hymxftah.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yuisyzxq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pcenbpcf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gtnumcxh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qwiflczz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2emfyamwa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ocfqdmad.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujogpdvr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxbldntw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mxrxkkkp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ndfkpvbz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2awunztap.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qrpfvwcv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pilwqbhg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pvlpvofp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mvuoeyrr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nfzgevrl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2srvotdar.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dhpnhkdd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hhumahti.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mdmihsrp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ekwcfana.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vniashyr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceuifqqj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2txulzemq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyngegli.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhjutxgm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aioauesy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2okuejazl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2spdzgkga.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rkkbvkze.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xoonortu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exepxxms.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2izsidgnx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ralpyifh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhkwjmee.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rwfmwcua.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wnznpngc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nsnnbjsi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcjozfkd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ypccomkv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2agrjgvwp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iibfefep.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rznazpae.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lhzxcpzd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ievyvxjf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2amzgnwyw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eiyuaebj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wyehcdsl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ldzzysbz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2aolycnoi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2faqysuwc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rqpcbetf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fujkxkep.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dltzrwci.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wwlynsze.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kmorqhvt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cfpvyvmu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2urdchtqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2uyoymekf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lpprblhh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xcobvtir.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jztrnaio.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cszmmttr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2josxlezm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gdiojptv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nufrkdoh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gsmakvxq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2prbrhayy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vxvwyors.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxbqhpng.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ygbyuntd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2guugdrmw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xrkwoeia.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wzthioob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjvttvdb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pgvwfzwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpwqejme.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qpzwwcaa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zesnughu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aorndhxt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gmknaqpy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mxnbsjuh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gizdkxgk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2clsaalre.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fyqxaomy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuhzfxyz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wggfwajr.html


<!-- 参考信息 -->