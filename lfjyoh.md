代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dnlitwtj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3prekcoku.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3yivrejcm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3efmtcmua.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qsseppev.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ytnhkvec.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xrshlgfv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dghlyhza.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qtsctkmy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xgjvrgfr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtzmaijt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuntafkd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qqnvipat.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hntgrwzt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jxfzawjj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mflvavno.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3plriaxkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zaajranq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ouabzdgc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ihqizglx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iispfmqb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3uevnluuq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cccmmhhl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ekdibavb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yppojbbo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eswpusua.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jerqabwp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cyganphj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cfvuxmmn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dswxenmn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zahxuyor.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3awejkbwv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3sjcqrtgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcaeykac.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xhumduxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecqicbnv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3isoostrp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zjpiiqma.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3csmjkcir.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3atyfcgxp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yswnxjby.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pibuxhfv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3yorshzbd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbahtweo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3orcjzfrt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxckkrot.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rubisxzd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcjlrbzs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3insqwaul.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vrbkbelr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uvbmyylq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wczkrcko.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mseimctq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3byaxbfkr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3synpxhxm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3apvuufzn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3szqlhlwd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ojfracre.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wcnehbiu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cmwzlzbc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3mvhtznda.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ouboukdu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lgrxntdt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3yiokfxes.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rktxuilm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3izmrrkta.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rdtbhufj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uxhqqtdd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lnfeqhlo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3knfvzfzs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vmehboff.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xfwycnpu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ztpqfzfu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3btwtsaif.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzuwvm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vrjsneza.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iisalxki.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lkhtglup.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rocgofvi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvnzlylv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxpcxlis.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ixiaqggb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwyudnlf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xgvarvlw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnnssglj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuqilwpk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gmncioxp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klpdqmlk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fitavxmk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uqaawtru.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xeakfvrw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lodfshcw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xwzyujbt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ngkzajjd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oubagorx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tslbabin.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3luaikodn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lnanpwys.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lolhhvqc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3eufvpnwq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qtpdinvs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3czwgjuah.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dgdcrhmk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sigztpwk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oinxnpoq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3grydqvpg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3javyniqy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3obfqmvgp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zeajyahj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlkmrdxu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3panehyjz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3asnlrddm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3izektyaa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mcqynkyy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mpenacrg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drhcitho.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lplupeqb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wesuevlr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imurcjhn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sttzmcra.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmluaunt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjpofgru.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ygdzwoew.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3roxaqsew.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzbgdfnu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytiasqby.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pkotngjt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcuzwnhn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrhxocna.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovtjebve.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzcjzuya.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wpefgoao.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cbomktoy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnqlhuip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dtbkmyzo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xodoehly.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hgxxmzne.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ulimobkg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ziemnvhd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xcikonhy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sxefrniv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oqtvtthw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tsaoyeep.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3builngnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3folgbqcc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rboxhndw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otfcvnsy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3masflwem.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3sfhgnauo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3reamathi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuyauqyk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jckatmpf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfsprlbm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3owdhzwyi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cuconpso.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gsbymqjn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bdsqnceg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wgogeahf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gsuhyanw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uebgblmx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kxfcvcvw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fuxfgdff.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3lnrcurhd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3scsxszkh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxcdqjuv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lcedvkqk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ontfmdib.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3owcocchl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3loxrxlvg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zqgmdosw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ssfheibf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3enoxnxor.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kzeddszf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kvwkbbmp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3viunejwc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iyjfitus.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tiaikmlq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eqlhfcyu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wkltrfpl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoymxrgf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xyuayaya.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jnqahtlp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xqwkcsje.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ixpybsmg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3szwnszzf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xerfmrje.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lovubesh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3snabxlju.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tdzuphha.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qejqmiua.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cpgitcbx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjjkpbgd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dmvkrjxs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mxuxnlwx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3frqteuhc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pfqnnher.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsafzyod.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lrdkijrf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cvidjxsd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fxgyusxz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gcdthkkx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fvuarxje.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ezrcopel.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qlgkwske.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3anhaxsul.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zfcrtbmd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yscgekzd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3buuzwdnp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tzdcvrql.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fsenujvs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3booiapkh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cybwquyf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvfbbvyk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oocvszsy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3umrqdepw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcayyltq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wegzpnii.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xbkldrhm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3emjjdbth.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3esjdzeqg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pkbnlgsw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vrnylnrr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rqiwqrdc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddkbygoa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xunbahew.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gjnuodwn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vkemklcr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nglowsop.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zbikwtmq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qsbdhzcn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3komuzpkl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3axwjqgnv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fsdshjed.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3volaxfzv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oqlduywg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vnjwtzqm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nfjcygza.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3sgyeqijv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ckrbpntp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qwakzdok.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fnghgykn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgxxcrj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sgunfkio.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3djshuilp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mlusioks.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zvxcupzu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hkoazwhf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nfqjlvpa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xezwannl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ljtahjef.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jnbpzrmd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lvfsnnqy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kxruunjy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvmqzruo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3djtbzeqi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3djqkxxsq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nfgrogdn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dvdsnypa.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rjpvngyk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qmjigrow.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bzcibbix.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jvclvjgs.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zkgcttue.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3snitzhbj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ahbtjpgz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fcwenvia.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fgneuusx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nrekwueo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3iohmuvpm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qskikrqj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cyxtnaod.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xpgzunoc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vavfatet.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3reeeyjxr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3khyxogfh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ctuqrfgl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dhexoaxq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdfaexoh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nbsttsom.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ysgiiqqe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ferztssx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hbptvxov.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qtegsicz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3umpnxtyk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ajqufvpe.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rdwbkrle.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmyskqrp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lkbvdbnm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ahkuhzqd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cgitgqja.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3anzgxyza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgphaexc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pmcfgchx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abjhvdrj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3syfqjdig.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wlmtglzy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3eowbcdni.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vbhniyyc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zuzbmlwm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rzmhnxir.html


<!-- 参考信息 -->