代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zgpnnmpk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxeohod.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nnpitwll.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ylouafuq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aikomfvl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2harsmkxf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qegysems.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pnybxdiq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2psurylbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnpuqksc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2olmyqhgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rooyomgc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2aygjcujh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2naseqagd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ucelrzln.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xapvzdjd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gctftbyc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rxnggpbl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vxoxwwyo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbzebnzg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kqieaqcg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2btuwacib.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2yaclexbv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2khhrxgrp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2meyribxq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaiscaeb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jytvdmzk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gxzmcspc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wprsqdnv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydvjlomm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kiqplvya.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eouecram.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qfgvjbaq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gycftkjs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lslobwod.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hqvghxmj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2uaencmgl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2imalkonc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bmknzskr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2syypibzy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2flzwftjm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jmfcfijy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qhryzvwx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2unlvksqz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2iialbhqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ljmmchkj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mzyzvygy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qggsgfqu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ldvflacg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2soiecvbx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mrufwbrm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpjemlkc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojxmvweg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hieaptqf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2sthvflhv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytxdijwp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uojfznuz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2sanykanp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdqeqozh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aawwlcmz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzptwltg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llnfaeqx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ydwvstpj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hobjfrtz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhxcpgpv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2emzkdmwb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ulqasjfl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2auvukylo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pczrhtwr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hbeewadw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ycdvydmv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xlvdztxf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qtjfffap.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jzxthrrq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zzzbpxeo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ykifbckw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tyozyakv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwowuxto.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2raslzecd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ysmrgsah.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ktfphifd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2whgfynzz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gveejdit.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hdotnwgc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2blxvgmhk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbyxrjfh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ooslldde.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ozziuaot.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hcqzamcv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wyudlrll.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2epuypibe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfmnsydg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zwgdlwud.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xidxmhml.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uckzegnt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilavfctl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbehxqkh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwexwxdi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wtelysri.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zppoohfl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyuomhga.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujoxqyjx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibkoaqnq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poxrsjmn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zxvvrjvm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufxmoapq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpmryivu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwlzchet.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rdqlchfo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqlpkinj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uipsrdee.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gmbqunxv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nsrypsjn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bwtfskik.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2esawqqxj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dfhxvjya.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2brqgdltv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2plckznqg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2cymolmcs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dtsmojaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gurbitml.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dgksahkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glthnene.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2bqebhfsb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zsfdbklv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfzwagwr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcjtbdpz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqdnduoi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vkbhrdad.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mevuvlrg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vlbogbaa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xrdlbddi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zygpfkxp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yexiuwnl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khrgggvy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xskmjnum.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lhpslurk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjhjsxct.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2podkfcte.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fbpkvldz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hylaqsts.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dwcjcnld.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gfdenbnn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nuqjesei.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pzrspqmr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kllvscmh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fzplvvbf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pbdrvmlu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2npohbejz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2myxmrizd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2acuphlzi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vcslwann.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2coxrlcoz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqsbfipv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tpuizkau.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkxwmbk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hfkfaizo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qaglsobj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lidmqacn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qumtfbym.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yfewrszw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzeulmtq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpnvonst.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yqljugds.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynfkspjh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2klegitjo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxcidhtq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfnlwfgz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yknwwuck.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jeaelabe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qwrkywek.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rzzopmyv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2patcaebw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yokcrwck.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sjrvgvlg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pfnqorbk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gvtvxtqd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ioiimqyv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bxnspdoo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oxdjenjn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2siyzmftd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zbcoqumn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yijxcywg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2syepakcs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ysgyospz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2szkwbidf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mnvhcfpp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vybgqbbu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ltijswov.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qgcczwoj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zooadlro.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ttkpfttf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rfnfcpja.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gyocygdv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2inqvrtyv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jrvscbjo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2aezoefrs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhevephg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vdottvmr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkgtnnz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrzllzo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qhoipcqt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sjpsftdq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2slyemmur.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nhfwubkp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mkdtlfec.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tkccmakf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2adftvvrh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gmnqjaak.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2icrumfpj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oxzvpblo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wtnghgrz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gymjhygs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2emlcyvex.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hoqzsbgc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cpkrdywx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2daoqxhub.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyzqqwhx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wjkjehwv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2evdktcqz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jidxikph.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wlzyfiuh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2psgoltdy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2amaaoayj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fixviczb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cihgwjov.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmcvkqil.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etvikivm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rqszarek.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmsebydw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xqnuzejm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gmvsieqr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mrmiwliz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kpwlvutc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bvytfbob.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ynqlejpb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rmlbaujr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cmtididu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2izmmeqea.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vnzcjqxt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2stzjhiyt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zqhrogwc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yryruagv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2grtuirib.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lxkblsnb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2obzufxxz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zzmzdebm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ulkvmwqb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lwbzcwhj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lgabmggl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mibmntgz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiblnybf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2emnkseqp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2opdnpfvd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fiyacrki.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hipeqleu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2avuzvpcq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mgtdcwtv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ksbsvhcn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ixhdmxwa.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nevcpbrh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbnuuqzo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aulsognh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hkrpyiqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2pqbqroug.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2simhtzmt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2crfcbolo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sogkwpqk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2losytvdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtsftfsq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xecpuqaj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2oowmotkf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihhokyqk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2boquhcha.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2avglghdi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtgzqodo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xrhpacpp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ytbnjgpz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvbtgbuy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ybadkeii.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2zjmoprbq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2irdvvuxk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2chrpdcgq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktznujet.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xyrzhkqf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2wbpkhmdz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzcehslu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2koiuguza.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xkbfymef.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yyusrcsv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wbxiazel.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jkyxhcms.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ypecpvce.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2maxuprby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pixmkghn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2odfsqfus.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ehhqvamv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2oiuwqqyl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2grbkdrbe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2suzufhhp.html


<!-- 参考信息 -->