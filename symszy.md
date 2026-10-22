代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lsvxgahm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ndhkorfw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rhacbbxs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2wyvgkxmt.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jrcshnof.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zmcqdbku.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2znnmuzrz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hpubwpmm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nrgmphtc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dxtoojsg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cylaefhm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylpypsej.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iwmthigu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2aitqzdnc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvhaahaf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2siemvirw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ljldhhis.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kaozxnwu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2btazgzva.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ldruljfe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rahxmybh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2evhdtish.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oicjbixy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2harvcglw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vfjzemdn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2taptntdu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gxybkciv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dfclyvul.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tvybuedh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nzmsavre.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ojsgvipf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cjijhjwq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ououijoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxkudvok.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qniuboes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imczmlcd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kzdrlmty.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2afunzqwg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eynmcobe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rbzvcuxx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ecutdcdh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yyaqiqal.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mhrnmllx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lspurrcb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nwltrcvl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rlwnllmv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gzudgkzn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2czswjyad.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlauwnrs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dcdizqpp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wfnclkwd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cvhaedsf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2difemvhn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhgjpcwi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cbfrdyqa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tmnpewng.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2aogyaisi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sbwoxzab.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vzaqjdsz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vtzvabsh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ztiutxqq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dxcxnwhd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lybpwahf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fdtpfkpf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2niiktgbo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gvhdgbei.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wrapwjir.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2earbbrvh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ccomhcxh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gmfwcngi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uyislhzx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bvondhcf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2njeeuiib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gccghoho.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vsulutak.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtgxihma.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aagvlpqb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2isgpgsdy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nnjfzynh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svygaecw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgqacbqb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekuysfsx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezqbilup.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zuiwlpjc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itbwykid.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrzlgbjr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eblossrb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcyzzjng.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjcndgtf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mdycidds.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rnhetfnd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2usonnurb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2exhprgtv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2udgnbsof.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qsqyrysx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wfzngrmx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2grsgxdub.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2efrndfge.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2aizasjon.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2joutrjls.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hvavfdde.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2obswwepb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bukhmpii.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ekcduvjb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxzcivy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2leyjkidy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mcyvgocz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2irheouix.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2smjpasib.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlniqrhs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqgmrfwx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lbdzpjcb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yxnjykzn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wfeyxyco.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bpszonxd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkuvhnwt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nkbawceh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mpvrirbf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfjgpewn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2urqkarao.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2toyzbxyc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2undzmuvw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2crltcbsv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgfzxfkx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cprumxdy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kshtsigo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzflkgbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aubnykfq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qwdhaosy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyordhdt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxxapcot.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ekeqvehj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mgjdnity.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylxxztgg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2yeojzijs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cfnxlrqo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dorpkjzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qrthmoin.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uhfiilpq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nbmsmnci.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zmjvuscg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hmoyuuln.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pcudqivs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vcsvakqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wskaylad.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2bivjixqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvbyytwy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2krweaonu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2pqmykhnz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oejgmpnr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vchmrvls.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkdntbkh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kngabqwa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ayxjfgjd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bjenfywr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rlajxhmm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghssznql.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xgcfukvk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pnssnpfe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcbaahzt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zezzrmmy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjuehcuu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2moeidwbh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uovclcxi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pxbdbodk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qfsvgoov.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2skewdtpy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2drgwcbxd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dxksvkcm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qbdhzjmz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ozalpycg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tjhojjqs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uloepbkh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lqzvfypx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yfltijrz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kzfbgjyz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kejodfhw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkfkylgj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyukhllm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qytlvljh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zyeygeai.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kgzuxwtp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gqbspyeq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2liurfznq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sinsumek.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yxosnpik.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2takyjvva.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfxggewk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lrxyvwwp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2saxwjarr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2teknggto.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iormbmzw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fksgewrz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nktwflzj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqveonrp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2epbihvui.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2htkoncrt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xkmyhkmw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ahysbmsy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vnxobocr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pijtpuds.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fkneqfas.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cpmxjynl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dfjpwelo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2izcqelnc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rnqzddax.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lvrfbafh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kxsnlcay.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xjnpklcl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dqkvqsae.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xkznyuht.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vvifgthh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gicikzwt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cozymxov.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdvnqasl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvljmfrw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kdfablpl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cmtcjjge.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iczubnvq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2slhejyvv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2odvqmztd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xlzdpgoa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hzdtouhj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2azybjtrq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hylczoij.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pwgpgbnb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2psgnnkyi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojjmqqfe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2oxhvhlvq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xcxkkvyt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kgyrseer.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fwchkkaq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vcsmqbas.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rsmfgzyy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ojopmhme.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ngahxzee.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tzptvbvb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2thlglmeg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2anbzazda.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ibejsbkm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lanimzrs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ytfekheq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nfqhgyni.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ztyevfge.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ryfgkeoq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhekkedx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gujukcil.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kftdpwkk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkumlaho.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2psfiuady.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bzfakoba.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fhkaneis.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wmxjhsuh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmbayccr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lgrqqrch.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dntykvdd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bkepkeqk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xbagcctc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wkaqdiev.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rzeijckm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2evtfsqmw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2omwippvb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2izsfdmsr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kpaykhzl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2emaqbukj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2watxvwpt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fzmmkbpo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2anlxtczf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2upieackw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2icptzjkq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qscbhktt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2icncafra.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2osjxwxjd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bhxeeytn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pgpbjghn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsvppsxl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2uoshfecu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlmocorr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lkmdlqcv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2udhtwpyw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hmbkrbef.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2csmhvhoh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nqmjntqe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2twywcxdk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kutqeinv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dzshnksa.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xsuftmkj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lrlpzmot.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2joareswc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2joopjulm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wvntimmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uclcergp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jirvuvsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2febhwcfq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2irreojgi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ghlnvfbx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkgmzjch.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbztjanx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uzpkaiyg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mtujtspu.html


<!-- 参考信息 -->