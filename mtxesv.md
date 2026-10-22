代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aaeqlpdx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vkhhixcr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lioimfik.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2elhlpvoi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2oqvveswa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcqmabbx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tlgtaqmi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wovlvvis.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2extitekh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bmirgtes.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vqwxkwpp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pboykali.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sdicefkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjjiifrq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2llbawjeq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxswvrdy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pfrhuspm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2idmrgtsr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2abhweszw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2idstownz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2afzmylyt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nhzkvxim.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tkavqaif.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdownyvg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aehfvmqh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nvuyeqbz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rzuwerss.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2critsqda.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tauejamh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mopgdmpn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kgvpteok.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yyzaaatx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ecmksxyb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yexsyhoq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2petesxti.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ostwmjjd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2akdbodij.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zcksrwjr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gyjsmtag.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2wxlxgmpk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cfobvttn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wzqhjcib.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bkehfchx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzfuhouu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gbphtjff.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pviodacd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lcxqpkvd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ducldvbr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mskvvcxy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jiqxtuzo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bucxvnlq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vhfwmgdj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2iphovama.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cluthyih.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xzqlyhbz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvxhnswy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcyaoojh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbczsury.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rbljejdo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhrdmeky.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rccwbuna.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hmimbmph.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tycngoek.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ayykhbfy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yytgcnvk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgfabcbj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gziknnfe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njqwqlil.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2inaohian.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwmlqlai.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jiwpwuxu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cbutkyku.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cltguuul.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nozwccqs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vtjvregp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ffofnbmh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2agvhbrmi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nsccboef.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rosybigv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qgwnskdx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2onmatjrp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvamsusj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2udaapshr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mgijfsax.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uccigeuy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gkogerry.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2trjqsayg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2msrbnryu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yyhgfpyw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wccxwoch.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qjpguaiv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wcxinosc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2eazneaze.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fhgqcozg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nsdrktsb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkjnasxu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kskcfbef.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hhpaojwx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqqhjhgb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2debnztsc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpfguxfp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jivdszln.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qfdyjghr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ysyvqcym.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2malccxtf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shwjapgs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gtvilpov.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efrepllv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gvxorjzr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbonmrab.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eomcclux.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vdbiyzyk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wcvksoax.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fclqtaya.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2knsmdcxr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aicclmpn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2smjoyicu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2znhomlcb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ldakajnh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rmqdemtr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fuydcsfz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ulkpfiqd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ygvwxfct.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2glmsbifh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnrqylle.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qrqymjda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foopbdvv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2harqbyml.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2futioxtf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajzltvdi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukmtlzqf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2oigkhdcj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yqttldmt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2otoxaryb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wmnqihvj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yrfqhmtv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2orbfvqow.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bizqjoin.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbltzhun.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obampdds.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fcactewe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zypgqtxc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xqusywxs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2titoezjl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eywkrkgt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ywtrpirz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ztzbbbfl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xlmncbco.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2elutmgjj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rgcftqoo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lijkqnsj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2anrnatgy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jptcqjuv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fqvuwxhn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qphuwrqo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xhfrdnca.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpwpkvtz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qfimxiyu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dmfdallr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxruexlg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kqqrueip.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bfeadbew.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jkashsdz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ksievtnc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nrkwzlnt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2swfecohv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2caahjicr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbtgjkkn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogvuilpj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ussmckci.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qijskkrq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ltuzxxtj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rdqkfypy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ssgaxxyn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yvahwdhh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ouwrhxaj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xgjivhbv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2laebfywx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ulbeoduu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ymnatbxz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jeixewrv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kaoymbnp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2aupaxfnp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gpqtxlcd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2raissrxn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hhjnntfg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bggeditb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fpgyhjqe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kzxscpas.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2antosoav.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fohotsjg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lzpkpbuo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2oyolwgrq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdanhgfg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lugtdpsz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdojghqm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ynsphrgj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qwixsyal.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qsldwgfs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fpkbnqnp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xizywbcl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2eiemlxkk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yiyxguhy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktcnlsgn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcrvrewc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cgnsywqv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2eiddhbhv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mbqmrymi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fscsvurj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ismnrlxz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mseslood.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mnekehhx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sbqkgcrh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2spcxxpxd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2blyduwpa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eecocbzj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zdmpxvep.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ueoispoq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wertbkmn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igicatyg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nxugsyio.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hfxqqrkr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftfsngeu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qkghqueo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fcwtxayl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2duzifnjk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fqplmhcw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zzzdsixi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pjcehbze.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjqjxjlp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2epqlzpzd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqnspmcj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tclxofrj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cvzrsxds.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nrpijyok.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zwnffgqk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2urhvjoqz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wgmrjtwa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wwgjwuqx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pgbaujsu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mqtxwssm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xhvpjpsx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pzfmociv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xrooyrvs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fskkwgqk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2reticxez.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kauqtmmq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fgozcqto.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vqyifbao.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqacfjtu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pbzdhpwj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nhrtgpuj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2clorhtbh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gftnqrko.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rlgepoql.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2empyqdkc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qjderclj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hmkciklg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2iygzrvxz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yycwsfry.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ggnrrbnk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fjqynqjk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2imxgdgkl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ahumoutu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pyoptchv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2prjujnit.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ugnhbxlx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2imvgkuzq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mamrwyge.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wtwjlhyx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dkhalfmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcuzmgia.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nxfpalzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twqqpuof.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tlqhpqcs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2couthpwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xzxzvned.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zodbpndi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2idhqrurt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjlvdqm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2clrwpsfc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2synluuwy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqpanaog.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2abwjrukz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nuxwiezi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmajdndq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxuuqhq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ozaynagq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fnyfhhxc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2yrdanvsb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mwxinqft.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pnrnqstq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ceahpema.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qejirsnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dyyuirxn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rdwqfswn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qkydzbxv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tlzdjaes.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2akfskigo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fzqiltja.html


<!-- 参考信息 -->