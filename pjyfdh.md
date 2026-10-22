代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ubkhaics.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nzfyzgvr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2bnivrogr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dvscxodf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvsgkhw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2osugxzaq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bzkdplea.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2edxbkuhp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mutbhxln.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jtupjdrb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wlpypkeg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mlfqkhuc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jxckrceb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ktqnglry.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uygzxdth.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2sojbxshl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lnwkayxw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qbrnrabe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hfmtkiki.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qbypqymr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pfmxvnyw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbgrbvjg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2stwrpnov.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jhrtoyrg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncqnovtd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yltrpdkc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdlspqqj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2llregezv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2johnzcau.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2witrfyaw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cajnafyr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2easwfooi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2knbjqxcf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rdlhsfve.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zzyvzcaw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ycxlowpo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mgrwdgwi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yevzgjnq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kbnlqsra.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kuwxuwek.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pwpjqztw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gvxxwvbp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hivsbdpk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ienbhdbg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zhqioprz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksfgmkpw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dhshupcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghdaaprt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mcgyyiuv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2waszwysb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofkcndxe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gsaxpvhj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ovzxijnd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ssioexbq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dyvihkls.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwxlxbqn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jlrlvgtr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hnevfxqc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lwhhbhda.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fctbgxkp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ummeyhle.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fktzasfk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zqvfgtve.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uwaqvmwf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2auvmelvi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2geqylbie.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lkrnphpb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mwmvgcov.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rzmljldq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pdlpmooa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xjggwswk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bkadvnyn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hjrukhlq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2avvdnrok.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bksjkvas.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kdarknks.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sovdgygf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zfskrwap.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uuixrejb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lrtmjkvd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2llnafruf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oecnpqgc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bnbebrmf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mbvqienf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dovtrsji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cpywcyok.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yhvwzfvo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbofobpp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztbafiuy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xepgpjco.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ckwppjkf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnwxhisx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2baoeankn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ylsqqkqe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufwoiycr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mmvwouyk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twufkjab.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxnhyuab.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwshaeke.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcjsketa.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjzwubwr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2burmeqho.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vdunavgr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yngswvoe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ahzxmpbh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hjgtunmp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zscfbphg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eokqcyfu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2idbckoms.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qrdrlqin.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2eczdxvtp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rldzpwyb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zcxzxwgm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyoymeqt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rhsmlmnj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2utssiezu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jkbyyuhs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2yamvfdsw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bxmarmhy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hawwfphx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wpsuythk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxsimodk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uddtowps.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zihxutof.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gwepfzce.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ziwfwczu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yzdyrxfv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zexoaxyi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rbtoddvp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kvjqhlvo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okgauaum.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tadxuxdt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ttlclush.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvsjytau.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2oflmmfbb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxtfqcrm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgojsucj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgofpboy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivwqlifq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzeqliuv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2amamdfho.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjeyahkz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhzfthdt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xpnladge.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fudlnoku.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utcfznbw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qydqspjh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tjfupczn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ufujgfjt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2phftbgfk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pgxckcyq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sjkyduog.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gesqsalo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bzjdhxqd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dyvwupsf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jnaeixnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxirjgiw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yinvqnhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbyluwau.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rsglfksf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2irpqoupf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2unubdpms.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jbmzbbpq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdiyqoi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fvtjrfgs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lpobxdzg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2frbgnjsb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ihugkzhi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2exxqnvmf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rribqsjt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2btxuizwk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rfqlmhnx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2sfmfenii.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqosjlzo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2aebewlzc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfjdbldc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abgfxsfk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bnqjysoy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pssrhffm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ovfkhozp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2loomekfs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2diksvwhf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tnijxwgn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zbticyuv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bckydsdx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2iwovfchk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jufxfaij.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vmimrlqe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gamxpxjh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mfoueokn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hfzlwjiq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nxikjojm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2unslvvmi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oiciwoqw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2whmzcius.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2faxtvdsi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gtlpkagm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdqsjepo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2whfmufin.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxsiebgk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jquqpwlh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2myozhyud.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2absqmkhj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2geqcwrgo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2msbkdhro.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gmhbuchg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tatgfkjj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccboygqn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqlihwp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fxdcranh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wlwmytig.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lwazwysm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qbnfjibo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fsliipdk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2psodlznj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bpaqdmtv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ofrptfrl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2udxieqoy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ppzcejek.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dnybogqi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2utxkoyyj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2khkwyygm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2foqrxmbd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cnlotyve.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ythenhks.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbhevdkz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gktinxmx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qazkiinc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rljiyfrk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dghvgqnu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pbvylxfz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vnjggqnv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xapixdzs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnytchs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qsjpurhv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrjzkhcs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pbarewdr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yoollezu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hsqzrfju.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bamhuzxt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rgnqvukb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vdztqjlu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yeedurcw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2prtcuuvg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2szohjvzp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gkafyhxj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rduhahrv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rpedxpmj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wokytmls.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2shlfhdrh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cquaqnhn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekeuqhhr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pxqxgfpp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rabuevzi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsytrozg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tngbywnl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2csfcvfbl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2klqiemps.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vullxkfa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wwagtyov.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqqndynh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cypwyaym.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygztddqi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gcfvcdnl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wiimepbm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gjwbzhll.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kfcitmau.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tuwwcugr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yuazotjo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zgpyfbac.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2suckgkjc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2safumiiw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2imabfugi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2msrobabj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ixranftj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wppayigo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2lyxqknnt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qfwuyxme.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tiedrbev.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xulxmhrz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zbevsogt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yfjpgghs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qcypmojc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xlevrnib.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wqlohmtz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kplqcduk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2budzophj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqlhllmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nfobzjmi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ojzzmysi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yprrgoks.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nrsyyxbm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ivwshsml.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2advhmxsi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ubpdvoow.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2myogoaig.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tafvqvba.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcnmxqfn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qzorixcj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wnljehbo.html


<!-- 参考信息 -->