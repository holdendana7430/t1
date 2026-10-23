代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ddvwjzbq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mxcbaqxg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qizjfnmi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ejedlhla.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3libfatfx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rjtujtfk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dyuyctvm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ufkrvrrr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zhxpqcrq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wptmqivd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qjazelya.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gykyqywc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3siuiuxzp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcyzaaeq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jpvbyidp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ujnyawpg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jswyvhrt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cuqtrmjo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tszgyvgf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wmdvlxfq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sztmbpeu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kesfvctv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zbqibetw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3blhmwjep.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ygautgiw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ekvldfeq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qitraafn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gwjhgtja.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ymowuehc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wideofhp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mzirjeon.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zdnnrpnu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uqmuhorq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3antlmfyb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3buiuaegx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3renfcsml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ktdtwqwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtakxhdl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jezlmvsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooswdzjd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xtdblrbx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zumstrjt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gobkrqyy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hmnixqhz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aljfzrow.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tusrzvrm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3eihdvtra.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkjqaipv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xawbuxls.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jbiiwkai.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jqvxgvnp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dzdohpbs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwdcwqrw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdfkiapx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3trxyzspr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3aaidwbaa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sqzfigto.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ndvvspok.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rurflidf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cgmmhkdu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ilkaixzk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gnrufjoo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3apowmzyr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yyjigqfc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3aeidtmrb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fvgpfkpw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fqucchqb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rpeagrcw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kqscrtrd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ujkkvavy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tqhiwbwh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ojbzngzj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qgbuuxvx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gzjlqsqg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rtnoibpp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ejirdezl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tenimnul.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ibprbncj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mcpjmtwt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwpfhpha.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwdufrdz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bssfzmau.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kqfnujgw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gddohtot.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fybesucc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vtzgpwcq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttgdzlrg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pvktmlnw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewirukzy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mszzvzda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3drspewfm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvrfvnoj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwvzulav.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rgqkdxwl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3avsfzcuw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3skbhduos.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ptydyzml.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xeyfsbsd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gjgzoqbv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hqobwdjl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fyttxvmb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3agwkhehh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wlzdzwbq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ddgydumj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mmjotzxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wztunlzy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vqrusquf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jxdndrtv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3orvtobqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xxqiluif.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bpmeihci.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fykqcpre.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kapezjoj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xguvcpmr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbilenkt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gaakvgsb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3clkqezlg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yzxboslt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3frqrcdwq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtpeqria.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xhunkbpn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fvbmxzoz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acnuywpw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3awcziqit.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncwvqesk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsrkqqjp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tnqstoaw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pruscwhq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vuvacslz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbpxmqqf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vqszscho.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtisedts.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kvdiiyov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqjgnfng.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrojoxdg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3luzbrshi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rixmwlmz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3unjlqfcv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dmgbsqcp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lrpzeckt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uxjojnug.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3nptfvtwz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3msjgzzkq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3egepmadh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ispmwztp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tturfadg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dtimnklp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vuarjexr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asjoywzz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pivokals.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtzshbqa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xrafqqxn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lvoujsws.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bqzsrvwl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3serxcowv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3snpbsgeq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3oikqutxs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3potkbxvo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3byejyeqy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3biuqoccn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3auenksro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xfemdrzt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jnsogibw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3stbeblqv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3phwauguu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwqkowtz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3odlkhjhl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hoiryqvc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyatncpc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zlmpztpq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xtipeffz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3evxbllgu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zrnhzoqf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vvbhwctw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cwjfuwvg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3npdonahw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3temooves.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kwjuibeg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3azuczhgi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3quaryltj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmhstmgh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjucfdlk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3idsxehda.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dayjlqfa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ansldckc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nonhnfqe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hnprkifd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nchifake.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kxwjszmi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqkfmrse.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipeuzvvh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgmbimub.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjipxbib.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ebppgutp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fmceefee.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rhsyxeng.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kazrusae.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bxrhbwkp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oowliiqs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijrmzgnm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfsvvleo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ykafzqxc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xvpxtmpc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gloiyubk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rhaltgnc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yfzphant.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lanhmhls.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uewelphm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hjvirhft.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lcqcmyvi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cmbhqzow.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3aobduqyo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tbrhjyyn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egscdtjc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rgwlinpc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tgbhzhfc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hkagrlto.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yefhjkdx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jahvbqfj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlivmeqn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mrzfmwwj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3heijldkj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3umetnzyz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qxbbzpss.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mgpplhxq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnatgdgz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vhbxjaym.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qnczksrj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evafggrv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pyjqbxsy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqwycrhm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tyzqhfiy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3deqzsbwi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tzdikkmc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sdoruodb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rjvrssfm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vsszvvtn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ciypnkrn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ezwadeqw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qxgffavy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pgluxdcj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gdjxjmhy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3utuxxdbd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3quucxqaz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ypuyyvgu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3soynqknl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhednqoa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hkgexrjv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ggyukqtz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3piauvoyy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3imxisokm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nifppgqs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaxedwdi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgycoswp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icnjmsnn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uuvtkuhl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gwuonsvq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wwnbrvzx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zpadoxoz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3damcplhj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rzpyotpm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lkhnzbnn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jfpzfqnh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xlmsidyd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xadgtuff.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mvrptqxx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3niechzko.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tcapmdeh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fscprsju.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rrkaomue.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3djclsmkz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wuockdsb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3namkfssx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bbuvvhob.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ieifdytx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pkjisesy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fpqbrbog.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3fcogclaz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fawpnqty.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxdnxstt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kfusfzxi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztwwgphx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bgxzqhsw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhfymmh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vwkmxtgm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yipzmhkh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bhmwflmp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fakdrrat.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tyedqnbu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hyibweib.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3sjojyakq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gobstkhy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zevejmgq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pvggafbb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jykykhrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkshjkgu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fcfweief.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jggfxqnr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3afuwpqio.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3peoczsuu.html


<!-- 参考信息 -->