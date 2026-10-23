代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3msqjrgeg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ketabibq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qqamngcp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qcoqjlae.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3qniusttv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3htggyiey.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kltwkzwz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdxyluqc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hdvperqb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3trgirivp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlelrcgn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uhgebpiu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wkntfacf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3guauziad.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gdxnqjdx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wybqyrro.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ihgqqdys.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gywoepdu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lkuokpdk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hlaijbwv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ilamkdpl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3whijdvzv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zjymwuii.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kbtstrkb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hsgadebk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kcqlbrkf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3sgtrmtgw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sqhxxlwz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mmvexwoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnbtmwlm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ijtjwhga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mviqnsuw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3spjtdoaf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ezeqpkda.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3smmzzjin.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tfftqzse.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kjtzlizv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xxxbreqh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sbjsulhw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jikeqaoa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xshcsztk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ogmnsqdm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3chgevtoo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqlnzamp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xgvcpfea.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbqypjnm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cmvmlwsb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wpjvsndx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kowbtnho.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3crwzfusu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ncnakcln.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vbtbdmcj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gvtgtefm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xdkaxwgu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3prwhybgf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gjhctjmz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fwewctyb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wuvorptr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kfcjccvu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3draayzkf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pdmimxse.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rbcgimxf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cdunzkms.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qzdjykpm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wragugkn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ossmqjbl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3prpspaff.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3intmlptq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gpyjztof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jencdzfn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3opveajto.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrqgbqew.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxmruuoa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hyajzllb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mbdqukur.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqsuxgfn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjmvwkui.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bxrhbakq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhjbtpya.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qqeqfwll.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yflwqhph.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyesjlje.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cfdnolrn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhaekiej.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipemadjz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gffswwxv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ozguxhzb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vnezkvlj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3sthyyzvq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3phkjowjy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ebpeigwl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3apuxasoh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3iigchrpj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fxcajzaw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gowvepql.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rjtuvijs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3twaxihim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3loztosii.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ryutpdzy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tcdupoab.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkizjsn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wdoybndu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3itpkhcbq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mojavamo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jyhtxvch.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crlxlwrc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ichlbkfy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fizjbkoe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nyrxjbcw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ikjgortc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zyywdgqg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxdbimmd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hqysnynw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ryfkhypz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3epvjbljd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ggcootvi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ityxgqyw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifttwhov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vcgckhxq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfjweovb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtrybmwf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilucrcso.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vrxwfcqh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adqjrjoa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3drzymmrb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3foqjtckj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbbfrtol.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3apvjcuid.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nhlborbm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcjpvcmm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uvuratpb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3oyhekido.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jsxfukuo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ggrkmkst.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rwrgdthr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tcgeqxpk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3lpmynaqy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jsfutads.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ntmjggsc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gkxkgyrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njonajpe.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ftxolbou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwxksfba.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lbqfwyjz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hqifqrqs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skiwdrnk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xdyahrcd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyjofpm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xicymdbr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yjjfnmpy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vuhyqkyp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hxdmqymz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hulnmeob.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xqaqfrrn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3iyctzeuk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wdqlzqhd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zccwcwge.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dsjdeolf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xpmuinay.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ggqmthrn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yylknwfv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pdwzpacz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ghbjkslu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzbtxgvo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eajolbli.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dvlhzdov.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kujvbmxq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rczddvtq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xcrvucqo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3myooqhwp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mbjkrmvc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qazoldhg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dlcssurf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ubtpwphp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwaszgmn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zfkotlrj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3labjatod.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvrvfftc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bqqgfdhs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pkmvzjyy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kjxxeorx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpdxfkyo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3knjzdesv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifadnaan.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcrhexkw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3teyrkcvn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qheqeyav.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bpfgwlvd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dbuxmbsn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zbvvxkcf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fzxcexiw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkdelarb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3euewqtle.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ezhblptq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vwzfnjhs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bfdmmoht.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pdrcvqgs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3wniygdqe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3unxapjwy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qtxqahng.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcilnnwh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jkkseove.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aqliorye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hfmlsfko.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ymdnherf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zwqdspbg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ffztsbby.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3obqpfstu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vzgehjdw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tsczhshp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpqzsoxn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifddwvji.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bamgakyx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ahufvqbs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rixnoiei.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3clvgphuu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zknoniwk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yzvqcddi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hjhkcbxr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fjnsszlf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3czehvrag.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cgjayzuq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fshdinlc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dirghhtq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3safmqvqn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yrghxiqv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3akbqgako.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tgsamyyc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nfgticcc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nuhayefz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dauiwcjc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3naaprkuj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3swleuhfd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ptxrkacd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3otvxjrun.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnwwogxa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mymbvgla.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uktokrlc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3byqjqkku.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mgzwkodr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ahcadoid.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcquoyub.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zsbyqupj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fqxklemm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hlfjaqkg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3olslugwk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wtqdbked.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xtawjsdd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nawsvepz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xokwyech.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3onmnbzyv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uabicgbc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3okxdnowu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gwsvfxjz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cybotcoe.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xctpakld.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tqtbdmmd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mpazjwax.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mntsxvcs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pepwyiup.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jjqxekxx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vqpbfhyz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qiodqimx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mwkljqds.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3idqqpajm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vccxjijj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pithgrjd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xlnqkulj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nosokpqd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3axiyqpqx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yolyeptm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbqgyddk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3totmcfot.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xmqawuew.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sptynhpz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3aajbkqqw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zkhnlcyw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sfjcqxof.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dopzcdxq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3yqivknun.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dtyhdbph.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qizgejrh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gsxiyqsn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eutagicm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3dgjykccu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zzrqdwul.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mqcuxvuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byiolfvg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fbxhoycf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymlokdac.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bwfpsdoh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jmqcurry.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ozqhcswe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3peakqdea.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fodltzzj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3egnkcykc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bjbazoab.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3afpvzzdp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztjrdvgc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3siffmgke.html


<!-- 参考信息 -->