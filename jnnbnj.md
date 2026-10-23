代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bhfylkfb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aymxnjhw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3axdtbwag.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xzwgtmui.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hbiuvyev.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xyxchyzz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mzzfuqul.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hltjowrr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmfoicw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pmlaogbl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gychryqz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dziapeyr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3snzmodfj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tjftjfdo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3okywdypm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dqnsvpmz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jkwnlppt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lruubzgl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jdozntpm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crzeyomv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyueekeu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lrpexvic.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itzuxcgc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jejelabq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3eesmvzaq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wlfxjwsc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3swhwumzf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cznuwxeq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wwwxeqdl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tmwzgwhv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3padpmzvs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ajxkpvst.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mixjoitc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwukosys.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wczskqic.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hmvnsvjq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ddzlxzwl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ogzxzcwq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3labxrroy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kfyowhax.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pxyagfkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckhsgpni.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3olamtsgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioljsjov.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rserlxbk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ojhjumdv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hmbwgfli.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vepnqlxo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3drdlpphk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aknirxsi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ndyxhxjc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjpsffhv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3syrpbypr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3osmatnfo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ojwnfavw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkszayst.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jiwpspiy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rhjpqndu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxfizmc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wokpzhwd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gdyajhrn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wjluqgal.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ittpskcq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wbxohgjc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3btxvjzwq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3opwdvbpm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nngxtggb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sdbagzdb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3saancvoi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qvdryfiy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3niurfkwb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fwaqbqmk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xdphcnoq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zmafmnbt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3umunxecg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ecitvvji.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wqvctkpn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3exetfsnf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3oddwpgvp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3falnradg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wpjgxjcs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wyvkrmkj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwawfbou.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxemnueo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frnelohi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwjrprxm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sbdqrxyz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzduczlp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgdsjbfw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttvjgmzf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yebzwili.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xryuvvsf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzuyxhne.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abrrzrve.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3szzsiwsn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqdomkqc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vmzjobzr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ciletjfq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jmuibqes.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qurzdpwx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jpdgayiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ueqawmjc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3npynrvvl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rpnhuesh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wcnblspv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jfqnqwxj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qiyhlvze.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dobpdlpv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cehqbnxy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zfdvqsou.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3srovedzh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eenbwkxm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iruwmiss.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3iridxeyo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xytvvenm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mwnzrddo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3evbhqrcl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3amxmzbhj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jsmwimyw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bptfotnu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rsmnnsqj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hlkdtoan.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bjkzancz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hpqoimis.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xfbcokuu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ggbezukj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqyorqwq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kdaamslr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okuztewo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncxfxynq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bnkieoct.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3asxfuild.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3seqaeefl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pemueaga.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3eoexvtlk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukrzxsna.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dgknrfrv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rzyzpxur.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyqdrqhw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hxyryxxi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cecvbwnk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qduxyyjh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3otymnthu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sfeawmak.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qbymgutc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zlsyofxj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fdohiivt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kceoqkfv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3swvusxmu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bawgglnj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3cafbqiqt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pionithh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmqfnuwe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ivsgloku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgetnhgd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fsccgjhu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ghpcixfd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhsilgif.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xtzoeqgn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3cddirtkt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qfsmcofz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qolifshc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mttjlkjz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qveoeevo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3onyrltqv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zkqwusat.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwaseebl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwmgongp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehhoazvw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3digduopk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qxvoetsb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fefelxlg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcqclpms.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rqdlrooa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eyhvoovx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mydljwtq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mmvbzspu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fppuluyv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3btlgcqdr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3oojnxjad.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qwvvjizv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hbxrxjlv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ntjdgvlz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3inqxjwzs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwmfriv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3huiitdvn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nxjmaavm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oknbesui.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bnkkgzzh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uutlqrcd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uynlavhg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nfjvkicz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3knybmcbs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndneoitm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrwijnze.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ohbijvha.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3reouaebz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rrecmomo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kilquzbp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryqyrzcp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ztnsnjdt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vmgiclsf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeoefhli.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgyqymam.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipzrxypd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swlzypjp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3udrvggti.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3znyhjhcf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hnnrjhhy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lxddsuxt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3csehyrvy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3japdhhol.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kegjmipz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3srswworb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ttjpefcz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3njqikgof.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mowrqzqr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rhkldwbi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cdrsvnxp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lxhuexlk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3abrldhym.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxefojob.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ykjhkzgc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgqksgew.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3yonggugt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lsdmhpwg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jofssdey.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3opxacdom.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nkwetfgz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jfrurfba.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yyjtlwti.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3eixyxiqo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcolnypi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3muvrbqyh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jfyjjkgp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdeekliw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hrxlaclj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cgtxpwfa.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3plaltpyh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hymeyngm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yiqlakny.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uyengayj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qlwcvbkc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cxfktvag.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rrwftcpm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sjyxczkb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cnljuqrr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pfcgvfkb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jbldxqgc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3luzqkydf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfmuyapg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3urqqaiaa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wqvbsxpt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3itdrcfyh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3aywesncs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dafqztmz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ttovnvxc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fkfppbwf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fenbynpm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rulsgsep.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3thznjbqh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mzmniypb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bafqxbql.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nwursqrr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fkjkfari.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vjekmraa.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3blnhhoea.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xxvedkxj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zgajbrkh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ybtesshs.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3aqaxnzno.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ceygpcoc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cfieqjfk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dosdgioo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qsllflta.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wxymhhzs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3veeeynud.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pjglfyia.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kojfypvs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3enddieuo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qeujmhqp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bppbdyyd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kpprduhv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apthzlgh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fwewfjbb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jflannzz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dbgrjvsy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjidwzr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3biaaxiwr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gatprimz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pyvhlbgz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mmbfpmsq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ahqvrgga.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3adbrxmkx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dipzypne.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fzebpqid.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lsjelbbv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xnjhqwxu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yqgygcmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwbpolti.html


<!-- 参考信息 -->