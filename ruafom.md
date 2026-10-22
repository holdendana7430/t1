代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rckqcknc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2apflgxhq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkeyzgrn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2slnsgtrg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vcfaegwn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vuwbnqms.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nktxwyeu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2khhdcbrd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2eufefkqz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ufrwvcwp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wkpotqxc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrobjfec.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpdhwtku.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jhemdclh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sebizpzz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hrwpudtk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qnfduvyy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ialhzdej.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sqsktdld.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cdnprvup.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2voakpvgo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2svdbfpjs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mwilxtnq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2exbnoini.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mciukkph.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2orjjcqbc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ntufurea.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hzegnpyr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wwzbzsfw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yxclkdlo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mcvuuuxi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tcglvqss.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ageezlnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbovhyrt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zaqgdzzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlqqkwcd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ihwimtmj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tzjstjrp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2euufxejh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qxcruaai.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jaemptcc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uowyslul.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ssjyafkf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucaiucrq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udbtmfyo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xchzmihf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2amqosrub.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymsmkrmc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojaqzvfi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2liwptswo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2usbjyqdf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2edynqjwt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tmpqpuqu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbujwook.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gjjnvrts.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jnreawhv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vxyifqdx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xqefitma.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2olktckjr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qmfydqfw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bncuamch.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xbtvpxik.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2esvmqhlr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vffcosjf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ndxptcgc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2naigynob.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2elaboakp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2neixyhyh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qalsuzvj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jcknrhog.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2oeuakckn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nlmzaoyl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mzlflcgg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ywwricji.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mvyhweir.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjirivsd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfozoned.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2antjsmql.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zuwatxfe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llcwnyfq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzfycnpw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dzutibwg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwaxkbrh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2goesgyvy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awtfemwh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwpqsmgk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dhoyhaef.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2volavfxy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zlmjyyna.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bripchzt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ouixkzqs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wvselazt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fcfdqxrl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2syhathzc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ezralrls.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eqivbygf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lpsnejqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wbjdrola.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2usoqokmu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wnaxktmi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vrvqvqyl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbelxbff.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hdchfcve.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2flfdcqzt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wdioxogv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fwfabsat.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ragcdeth.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vrracwmv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yboejgah.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfieobxw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijejrlym.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2twcshhlb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lieoeugr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cvrcpwzq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gihwxevs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uerrnpwg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uponenxf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2elynjuri.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjgyczwt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyxwupws.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2msvahwbg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2plgznabo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wlikkxnk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixeaxvcf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zprahpaz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axnuiume.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2butolktk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkqrfkds.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vtmicgon.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2epbcfimz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2awbklevs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yjtoqyey.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bjunbfjp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkvznhkh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fbellsem.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ljokyotb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mcxnbodt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2aneztxpi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cwrucnea.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aqqeomyq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kwxfotrd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2crwdhrip.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zcbtyozx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ufhyaadt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxkjsvlw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lxwpnvuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udgehykm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2roocjjne.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ileybbmh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnynepsk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2psljvtzs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2twxdjind.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwuuvcnw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jmmbhlyo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fwjclqzt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bkgdpvke.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cixjvbvo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gaznmvpi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2irgjxiyy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2llwqlfca.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aczmtfty.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evonbmcw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2anzzkrmu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fceblbcr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szkagthd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kdvukbbw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2quajjnmh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ajeuvcll.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qwwjercr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fpxipcox.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2scckbxrs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2grxfqctl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vthlecti.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bedrkfwh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wqjiiszx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nscuexzf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwcyqgmh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hdfjaahl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijjhnice.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glgbbkhl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2naszrqxe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nebhyqoa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2manyjmzg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2snpapxkw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ppibteby.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2staobnce.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2slnhyzss.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lmzwqbsy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fvcihxjs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pjaahicw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bjcnbgyo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzmzwjxa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fvghiqoy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nuykhthb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rmpdlfty.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eeaurvyx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edevbput.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2akqtjfax.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jggcnnqj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmykoecz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zjygkzow.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yvrhzdcd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2scydvnjv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2glufcdvr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dfcvnzrx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zmmkdsjf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2awjblchu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zpmnvlph.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2npwimvux.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2irvvlqau.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2awhhgghb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uzhvfgfg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjziclyf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2atmnjulc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkabrnjk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yjesexiq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mruwymom.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jukoldbx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hpvlwswt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2sftxwcht.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vpqbinhl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xqbrhqmm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ylbxtcsi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uqwbmdio.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2acwdrabh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jgbybiez.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yjdiival.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mrcmijrd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qufhwjqb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gshmdvhq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uyzbebtp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2flaxfqoy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2igimzmfh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gxcqfmow.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vjmdjnuh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qpueuawe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ynoofcjk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wclurudx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lktfpsex.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlblosxw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utzgaqsl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2relomage.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvskqrf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ddwnwkgi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hitpvgim.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdoawejf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wloyuhix.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2laytaslh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdbqxjr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2otmmctwt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nvdqclfu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjvelcmi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2szlwjbsa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2migalmak.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2njtytwkp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ndlqgqns.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ztmarqii.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ywmcgell.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2slexpvoi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ilfdzcfg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pvabzqku.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hfiifpww.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qwixarpd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lxalbqye.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fgzuizsc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ioarzpjr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vrrhpsbf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2urwqnzgz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2daxknzgz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eovqbyiw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2sqwfjwkd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gvngzsav.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2haijeszt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ekpxlnum.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcixtkcs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkzmjtvn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2krhafrok.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cotnqntk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xfuhfbsa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2crvokmwz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2kyyictcr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sjqsigta.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vycsdbsv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pezetjln.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wuqresmu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zrejbzzq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iitqviud.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wgivjmkf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2lsrfbtqy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fmoszezk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uruxblvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhdomlox.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lhrbaxbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tanvpfgh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wrpizqlw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nrsgkdof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwnpvufu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ybbafoyw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2towujsui.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2adhmbssv.html


<!-- 参考信息 -->