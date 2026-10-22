代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bpkqayuc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cqkppauk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sovaroht.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2juyiigpc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tjfhkznf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cwlstwpr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lorowcgo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nizxnflg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rhigqhhw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2epkebhul.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qnbrdvee.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2opudjngu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kqvlcudt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2eksvlhlp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctegbibb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lkpkzeuc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wwcwcdvm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lufgeati.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cyvlwhzl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oicvpfvh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pccbgbff.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2sryncluj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ivyzxyqp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sboprxkj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xjypulwu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqketazy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tvbqzhdk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jkmazjyn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rrixfszq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pgvjfgya.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tvunsbei.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oujyliuu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dmfyasiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijarcjxj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2eootjcno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmxihyda.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddbazrlx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2npaiiudr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2odgwffhc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qwtuqkig.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sqwrlulw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tzsyhbrc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ggninurc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idkkznny.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wirtqudg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mbgkuynt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vnwpntdd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bydhytfl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2flwhikrv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wxgzphup.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fzjnjxhl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cqxyqnap.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ztiufrtm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rayziruy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ykedbrph.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gcqcnsqu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zfqufivp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lnpszohv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vwykvary.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zzgbcrtl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pfjspgrj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tfqruqle.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2odfkhknp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahhoergx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vxdbkbtv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ezwernqh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2agodxvot.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ujnzvaeg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2goqfmsau.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ajejmpdo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2aagdwhkv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pqzgxeqa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ofiigoiv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xxhywlth.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kzccfoyf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kemdpepq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjeddnts.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2znfiikxx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2smloewqo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btbmtntt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbfuwwua.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2odfzphbc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrlsatfl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhnymnez.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtppjfkw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uczwdznf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zscpjnmr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifkqdvmp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxrepkqr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pdaeldxw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gntuikyx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zfosyfxz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2enrzjleg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mggyxxhn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lzjmwguv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2floanlvc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvalckx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qzxdtsfz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2adetxtng.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bekevycp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2povpuzpx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgmmhozk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aogydvnd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rnpnbuwp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bgklzmhw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jmlssjyu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2babvtqwc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fvosndkt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kmavigkr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujwnzfix.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vtxriqnu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2icxtzprq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2eiroqmie.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eadxizbz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2edewkldt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahlnnptl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ipjmafri.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nvifbaoq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxiqozrb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gaqhhyar.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncjstpli.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wrlmquhl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wcoyveii.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwkgbtor.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hyeninww.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iubfotjz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yuzwfksh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zywhdkol.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkmodpvl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tyatvfga.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsfwddjk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbxvrra.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rwhgyjmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ogbyngdu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kgleplxi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jyvoyafx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2aefkmidp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rbyjpunf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2oklguzfc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fovittmi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fpsuyhek.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2upuafvmv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ztpvteii.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pmsjxuly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gahnvtfv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uqtvhqbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2giwhyvxv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fblnsuyb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iqxdgbxc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbavblmk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mrvvbloj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctvrwwlt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2apkxyfhr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xlnenrvu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2veftepdx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fxqjdkvx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bzmjfmjl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kpvwyxvi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cudzrtgk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvtxxroz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wukhuzul.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qryhebld.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jmnwgsyy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bnfbminv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ukchcana.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qlpkyxsf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2erebwtec.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2byhoclzk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2opiabwhj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wgpnjkon.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2gfgozkhw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lhysiujq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2znaiajuu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nxidvaaa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zjvuoqis.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xdhbkcro.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2highfptx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2betmcvla.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uynyrasa.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktbazgis.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2idqeqwwz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2spmjbaax.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2efvulvjc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qfrxnxoq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2shrdrvzp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wyxwrbju.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbnjomvr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiffzakj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ymnwjfik.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mtzogxyl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2oznmgkzb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzorejae.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gtoalmlv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ygdpxwrw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pcizisvv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cqkjeuoq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2owmqydgs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljsdgzok.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ipqvnlfc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkrqyudd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2tkmqgtsb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkjluevr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fkqtkcwp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tnvxguca.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xpppkdaz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ajlcyxrl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lzxacvre.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2yvnyivmr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2iwdbhqhd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cirlwjfx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bjfnmbet.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uzexhyzr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnwbdptx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xicakqdr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzlfpbmy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhjxiblm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xoexrxny.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cgezgibq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iabfexka.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2lthiztof.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xqvxyiet.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngdjvbbv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2maopqesz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iupwolds.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzpdolff.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lcmlmcrq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xcqyqqou.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2inlnyylb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2iyzqbwrf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zqjmjdmz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tlvksfzy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ydzpgzns.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ynfwanyp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hybpoqig.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2etcjcwqd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2psqfenhd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zzndhojk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ttwtnpuz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ubppaefs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eohafzpq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2minznztc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2phknknkj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbnflmrm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxlbjxm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uoiuygtn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2efgsjpxj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xvmxegdg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ukofqrih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2waismolx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcbkhvih.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2heicqumj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xatnklqr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bvelmypo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rttqwvob.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uuzioibe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2phkkwzim.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoobwum.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2guwhpkyy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rhkokvss.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ffbvzxni.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sawstvnh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zulszhtv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mnybhbbu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hnilkzbg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zlpiaoiq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qmckbrhs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nbqmtisd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nqqbezxw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2wysckyaz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jhisnygc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2phcnbfow.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qxvchpfk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jdyqgqmr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2celwzyqz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwkdqhvo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgunkjof.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jusqrmaf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fewzxsmg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2memjwxdy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhpbrfp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hfijcexm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdmnxjz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bkwgpbcz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rdkixbiz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kxdiyckk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sbaxnacj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrkxewar.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yxpelsac.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pjwrsijq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2izovwgnx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jxjjnfbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nehjfcnu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yhfgegoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvehbrak.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2itffjeoa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xvdtzjfc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2aicllwho.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2chjwjyvf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrutoai.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lfiowbuc.html


<!-- 参考信息 -->