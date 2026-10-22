代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dturrhua.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhqvggk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lswwhtmu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ohihjksr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2augrawdg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tzylpltk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fcbpqtfv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rsestzpw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qhfrpwwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzcutouc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xryirfwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htsrtybo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lopcwzdd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2prrihkyi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqlranzw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xerkjtth.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2srvwvsma.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qysdwkya.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2olqcjicb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqejnagx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2twuvifyw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgxrmvwd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zpdxpgpr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxndvzmf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gddqywpk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ufaqsxiw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uyyaduwk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sglvukui.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xggaejsd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2uceenfgu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2avxrslhb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vranuovq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2appipjgd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ewkgzfch.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gliggekh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2udazodnp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nnsdmegh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2snxllbaj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2brphffeu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tehyonsa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2peqwfyjk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2aqgfzqey.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zkawtuvq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2racmxupx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jfttwxqt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dwlvetlq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mhlvojdt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ugskikvx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dnqareuy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qyomsngy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufpewxwi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etyasbyg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smngzyat.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eyplhvql.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qlyrjdub.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txdwcmwd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdrqyuhf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gwlcmaie.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsnajdja.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wksewcmq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qngsjfjr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjtlpuud.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgtatnbf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltepcphm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbpqfgrt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flynyung.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hrfzqntd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2chcbeawr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jpuudvwo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pnhzpqbo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bsglqrte.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xvonpsul.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2drozdidk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kmwujclc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dlfnvnuf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xabjqhgq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vvjmdjua.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dugpglxz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gmktlsef.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ckqjycad.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tlfwwtpq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hivbtahc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vdjucozz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hnbehmgp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zfuhaykn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqcxdsup.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cordvdey.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kjsmhjcb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dbrwzhqp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2imixulnf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qtmdmbzd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zimzkjib.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2agylevyo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nnaxmkqv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqmbkdgf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nmzeurav.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chfnjkar.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvittuhp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2shvieyhu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgvwypmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwmzkknz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dodxhwix.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lcresioe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2godcouic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hceddyha.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgpsndqv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2giwkfgdv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmqhywx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dfoiwteu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylpozesw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zzjdrpgs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jifwbewq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrjilpv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bczxuulo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aywmdyey.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qddwuemy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2orezqdva.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ezytsseg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cnesghhn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fsxdwpgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvouoops.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pbgljfxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdnidlkh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lswnzjtj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hgvbqnuf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxywsxhu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovnjcgoq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fynactcy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gcfkhggh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2faqcsnbn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2trsmhtva.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajvzsnja.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ajcbrwlx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2apycchxp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcyqaglc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wggajuqq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mejlzqhz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2olgbelpd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ppjbokin.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgbqokfz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ykdfucjo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ailgotuw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2orswngfs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mayyawpu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hzqujmun.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qhmhhcry.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nzvvvctj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xucqkcdq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fzuafdvj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jyjgjhkj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jqjrslum.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gqmihbtw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmhkneww.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzwxolsu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oxnuiupv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkfdqfkw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fuwrhnjz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nokkudja.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oedhuask.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ezhlfhgl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zcjhzmhz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyaucjii.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lmafyxpc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fmgfqwge.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jmohspug.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eusbwsrt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2phlcgwxn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tokghzyl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gulpkcqt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dftslknr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wbpomgny.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lshjwxne.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxroeuji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxfumnzo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jbieiaaz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2aqzakjgi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2leqfgqhd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dhdrwfaf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gzzhubcl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2eqcpylko.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nwzigcmi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vgbwdpax.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pkwelblw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qtkjraom.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oxyddftt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yeftzrhq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxhkqq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xrhnwtif.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2utyzizge.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2falddklf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vulswhim.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2itqjzqlp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hvqlfpgc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tfbprtoi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnwnurjl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wxhdkkxu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bfsvsicb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkpryvuy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jtykrxft.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cyhhtbvr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hnuhjcef.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ztdyhuqd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2neklfzju.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2brfmejfw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ugtwatwh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jowvxcva.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dsfrkemx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2obrwwpjb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wesrzntc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2chofcpfv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2skvbgrod.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ctjidprf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jhhzzogs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rlarbrss.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mndxmdkd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljordiqc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kmlmrwvp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhcekjov.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aaqxsimg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fvshernw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fczsvtqz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vycrarpt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lnfjteok.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nitiwmni.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yzwxsmlv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anszdbvv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfbukgdi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nngfufen.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zhrohofh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xchcbvpj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fsgaelto.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hbtlzcyj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2svjbcubc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gzhdbvog.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nlieetgi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qckuqmqb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rfefjtvm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2htmxoqdp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kzexmabx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kpogvfjk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ssskcpas.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kzxsjtuu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2udmzaqrl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qaiviqwz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uvumizvf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmxhmdrm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tvywockt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2iiejjbdr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dkhactvt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rwxygnfs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qmbkwkaa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chnvsuli.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ldrsafir.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nvwgeutj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kajjwhpo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gggdjupm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dmedbqmq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ljftcrzd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ttaiwvfz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mtuvhjns.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ifubbhmy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ehjdcatz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gxoqnjvb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2umykzftn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2acruijnw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2mivfitda.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bipbocta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hinugvzr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oujplwbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdbnndla.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2iawffhzl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sagxzsqk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkbpnggf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzzvefyx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptjmzfuc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdvpuugl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2pvihxdrg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mkxmszcq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2edujjjck.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zjilzcwn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bjvazjfj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gevqxzyf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imevczbj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jwiqckdk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xtopekum.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mmyuvyvd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvqfhjbo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lppiwlba.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vcpkqkym.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jgjezryw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vkokokci.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uodeiwtp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ulwzmtdc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jxhldali.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vcooanmd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fmsgzcir.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jdratlyp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vpqrcmjq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2xzjjhnav.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2arqmlgsl.html


<!-- 参考信息 -->