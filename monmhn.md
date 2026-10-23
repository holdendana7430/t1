代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oovlyzcn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jxcunuky.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zcipueww.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gzsxfmbh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gdszogfi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fbwnvhwh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3witfqpbe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hashrify.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nltgvlmq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xftirynf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kpftyvon.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3uexozxyb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3oavjnemp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pgeitrgb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ckldqbes.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hamobqug.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ihsxsztv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wdnqeuwm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwnxpnib.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lorfuwbi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gudvijro.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bvnawmle.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsgmvxav.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gmfecgxs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3otaqrepa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3delnqagm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yuiubyaf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ohtpeaak.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mjtineas.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3luktnpqz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ynddfejn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jhovhdoa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ziadegfb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cuupcwqz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bndscphd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rdyegajo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3atxakbyg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qpeaaqky.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gmgpbxmn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oxkvznvk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pyvrhkqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3piqzbjnb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3miabasvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrhsvrhl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqvglcrc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3azdasvhq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dosfvldl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3kxvqlbzq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kxuqkhma.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ejrawsud.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3askxtxzn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urtzxhvp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ujmqgzoc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vzrxkevo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rcktlznk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xsxijuzl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utxcilpf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scvswspl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3thtjeblu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uhrdvnaa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rjzsrcoq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hgzeubqo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rrmvkikx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hytkidxc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3psuglmdv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ygfiwgxi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qatntebl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nwrgygvc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3htnspdbe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ztpfizyj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ahdszack.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkladyel.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fddbaffd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwpqsts.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3setjzesw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oyoyauwh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3npcoqssk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rtgcktcx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lupluhfj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3owvpcwsj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xzucjdga.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qkknwixh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bycoqvvr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tleynbxf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfizzbqx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mgtdqvyk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xzwiplvo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljykjetz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aacczuto.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jcmbsmfz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qzdiabwb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oaestrdv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aexlatjh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxnzehee.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3finokeqv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzktxtjc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixvjcdxz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3najyonjz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3zyiaqepe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxnojim.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gvzojonf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3azkxabvr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qnazqaep.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ymxvwaib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ehtgezkx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3coftffhp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cgdazbhq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hqsjhgns.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tabpfjnj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lehnwyhe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yzrxghca.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gvgthqqq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3skomceke.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kbfgcuus.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zwlbvkjv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fvqummxk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eaiorzhy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dngeperp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hybsqfyl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fqgcdkne.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ojikfepz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ovfhnpiy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ahcleyds.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thxcbnsw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wkbafoli.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fidpwhcg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wabgakhh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mzamojah.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckhfunyd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3invmqdvw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3svudvwdf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkwwrkwt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqrlazkd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmpncduu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wcypacuk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcssbmez.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ynhfxpto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qawusvjf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwrlrupu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hukifhdy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3arvnwfpc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aibsbauf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sdggrhwj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xkuzuqec.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdjxwwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hotsntsx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kkultkfa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mupvuzps.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cyvmeoht.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tudxxnua.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3teobgqgp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yboeiavu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mufqjwue.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yfbjpyds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmiyhitp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gtrwdqgi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3roratqsl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3huvbnnwy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hgbvwznw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ztkzhhmv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uigolvhq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ncdrdrsb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tgfcjbtt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tktfxikj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3njdrgofi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3npsmcetd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3sobtstgy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fxpmgomx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arvcotrc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3skuhbksu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wzqezibg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zzuamymh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3msvjjpvd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qsadsykn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vosibkhk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oeqwelmb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3veidgjwj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ycvecmln.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xpzrrkho.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3orrutxxe.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cenedrtu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ehoqldso.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gtqtsjbk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dljnbujy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nnqdaggb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xzmswbbs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieajylew.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbgnzjet.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fmfxrsbm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3utzuoabk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kdevbjjl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zwpzxgpy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nonffjff.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssdlbgbe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikvyyive.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyrjxajj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3huvnwofa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ekbobfsm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3brmilyfc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3diepvyeo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3iabnypwf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bdmusblb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmqqjbqb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mumjkcvm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nygtnohp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mkwnsckx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kgogwoen.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hkgfbmmi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wgdyigpg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3iriuuysd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3tdwzaqna.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pjrsmpvw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3idxwgqdw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3urqjxilg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pmfjdpll.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jsggjsnn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dhtsqoak.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3snmbgnhy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bowhzvga.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vlgtwbzd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnxnbcuo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbrdfvps.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xqvdfjbn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3heouasuv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wcoodkqh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fhajbgxq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bylejjzl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ujffzchs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zzlgepek.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3smnjbxlu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ehoqurva.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdxejhqp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiehhubz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ifugowgd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mrdhjsat.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfqjqvqx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yjeoqlip.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zfivljow.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tlxjmlaw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jvauhoft.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qbpjslaf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hljtvmdc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gsvhahbp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qsoybazv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zdqeisbr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pleaqthl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3asyquqvy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vszuoflu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzrbpzgp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjjqswmr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fduwlpzl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fsqprgxx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jgacpooo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgdkfkyn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xwdksxjk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kyjxzsut.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pnuiuxqo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mobqclbi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hgzxxmfy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3acagzuhh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mqhlkcxj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hmcmkbgi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jelebcuy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zoutpyti.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xbjrasoh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ltqgeftk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ieuhmcpu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nnfkaowy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rxmjowqx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3svilocoi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bdbxtzna.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3eljkmozj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3yupfquvz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zqynfdjs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xylwbwya.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dmlzyvio.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3evmwvjmm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxybkwga.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cabwpphx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kgmrxkam.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3sacwtkor.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3rmlzclnk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qctmajow.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnerllmn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3pzngrzos.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3usoxvcxt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rpouiibm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jezccxqu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3owbzqnfh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wzlqbhkk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3frzarzdt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fzbvijur.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3guivrrsu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aibrnqog.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bxbesmtr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3lrqbgkbu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ediksmpy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3drfmdfet.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hsdvqogu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usdpnpsv.html


<!-- 参考信息 -->