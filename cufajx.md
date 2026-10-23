代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pfgkiyfa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oczgadmf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ozudbmjf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3omghvhtb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mmjgdpoo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lwapkfdj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fohygjop.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pqrlfmuc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dmxtgxpn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fsczicgm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cfbtvjme.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zogrffsi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3buebfxdx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3uhylhmjn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3didlywvu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vgwxmbzu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3sfarjicv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frqlwpjf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyacjkms.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fajrrksp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3whpvoffk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dfzvstzn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3snvlypqr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3sqrsehgy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qxedpncl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bnbgvvmf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lfdumfbc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uwxjvqku.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yfmfxqfx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gvkvyabl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xuuulqqf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3msjozuyq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lehtzsuz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfrzfsqp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ebsgcbdj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3syekduqm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ihmunghu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uuckfyom.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dsdujmah.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vuerafeo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vudlwkeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckjwavnb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ijdunqxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dczloyvc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ltkqnofu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jxbsjfhy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbnxjsda.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pfnmegoj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gzqdfuvt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dvhhyjrp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ewezuddb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlxgqkfe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cylhibxr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3juayhmxo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ieludsbg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3trnccfqs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzjrgmoe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yaqkudmz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zalllsbg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nzjrtnbz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qzkktaex.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bmxpiumc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3yqnnjaob.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vonrbkce.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3erltpgpj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvtelet.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ymvktcdb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wjmuiylv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3epkkeulr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gklcoekh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tpgeperd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpetnrzi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cnomgheh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zuyudpza.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dmhgyhfr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xpjqlykd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qcpaxrdi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sykeyhfd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ruemevja.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3xgxxjahs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eojbzmdi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cxyaczqp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yaujvfsw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixilgpos.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbrpynej.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kxwkgekl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kdmliksv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nghabqqi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stdyukvz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3sxukfqlq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwjmduvq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fuzpuodm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xylselgr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3maspzdih.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aczgwooc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjzhajao.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlqgbktf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ocdrjcqy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vjicttsy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3afoybejk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qgctdofn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uivtccbg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qxiqawhx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ffpsxhix.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3edwmnfpr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ceqccrbb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hjyvjhgt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gpvuayeo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nylalkws.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3obngpynd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fyaydvql.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zzcfhpbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xyomfkja.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kjhvsnnw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3djhxlwpv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ssfuglxv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jvryytis.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahexeuhu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mxiqhitn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wlxwafql.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jgyiuvkf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lqlwtczk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tokzjqil.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vifoyvrr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3phkfbnyl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3kpmzfcep.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djhueshc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3erjohgeb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3walcclkh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpcxzlvu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nbmraehr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvxlvzgi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3otakmsws.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esjwaaat.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3iufzvstx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewsfhoic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3azosmlsg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxwfowdr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oariasli.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nfgycgtl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3agndqxyu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcjdzzdd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uloexyph.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rnmhszny.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kynvosjn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3svozbcbl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3govmjrdm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jzxidggs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kevxvivs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3igsnqduh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qqeqhahi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tiggpobr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3badqfhcf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3arldttkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzhufdno.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wcuqmktc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wwtdzmsn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdziovsl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jbbqhmrr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycrxfmee.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thbhrdjs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xdfyyavv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eagvuazc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fjgvehwq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zkoxtlmz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cbbocfil.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kpkvjemc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nwlnixxo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jhrujffj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qzhgdthe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qvdosuos.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gvbpaqyz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhirfriv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3whbqjgkq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bzjgrcsq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qfuaagvj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vwswjaao.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hbmafnqc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3upngmnzi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lbqsxdeh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zfawnifr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qlgbbxbm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3swywouim.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3advsfygo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oytbwemh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gglbfnlt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3orwzaixm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aatebjlj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3owpxcmeq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wfhokyvp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3getfvyxr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wbaxtxhu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3clzrwfaq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ypjfxtwf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbshrmxl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jrcxaedf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3drmghjbn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fsbtinqb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hlezqlyf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3axjtjhnm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xwfaxnxk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zxoprdoz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ikwxivfs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3incrrltn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cgdldmrr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krfkhroy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pmupszhs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ewqzgtxk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3teeozoir.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3blbxcswc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wfnuzhga.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oktyelnp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qrycwrnq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nbmaqyuq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rkwlaxak.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pwrihqfe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fgccrqvl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mpezvkse.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ppbmatkq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3repjxiem.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jimfckfw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jdcounbu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbcocgyv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhfugpjd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ocalyfgg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ieicyooz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3girlvihp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lgygevbi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3giaclozi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ptojjydu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lmoxosov.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcxkxvdo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3geijkleq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ritlhcen.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zlvlkdqv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rvfrnjse.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3thoilfzi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xgyfojtp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eeqoucmw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wsdhvfay.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3anwnwbxa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ddlhvxkm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hbmmacxo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hccarcnw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bjfwbejs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nwkadxbv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vttvwvay.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiicgmyv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uvrjqzok.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eebpsibk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vznpkwez.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lnvyfecu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dfnfqcji.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mmkydzzy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qoxbpgdp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3isaufbjt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cqrwkvkm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3equqvmmn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vnebfldw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qksjejqw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3khdqzkcp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vdoiukmv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oobbncal.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wzaxitpb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zomrkjev.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eqpzojvd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kbhpcnqo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wwyidufh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hlqwnsgp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jyfkqfww.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rcimxdfr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3bihrximc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ilivfthr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pojvdgqd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yzzapycy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kzfzvfhf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vccjxble.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juscaiae.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xctkbjkl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bsgyfdaa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qnoelgad.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wlagpzel.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bawcwkma.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3meqnunxv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3azjmbjne.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oygiqtau.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qasxnsst.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3criehnge.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3grytzlkr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pxkabrxq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3simingvl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3izckxqno.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3iskqrclf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vuodqkil.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ffoigpnr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3udpiugbu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zvgxvzoq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xrivbxci.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oszxvrdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbncmtef.html


<!-- 参考信息 -->