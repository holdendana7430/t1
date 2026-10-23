代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xitrpzzg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oxzotjef.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rqgqqepa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vkthbcub.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3moxmsjkl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ujfmqijd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zspyoyqx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iessfpfo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dxhbiyrl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ifhcbfgl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ieexedze.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3uiegcpeb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wcfsmuwp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nloqukaa.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cbtgdeya.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3sevgdwow.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ztebmnyq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwreaqoa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3iimbkvku.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uhyavhwh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwxkjoay.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3moxrqhxv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kdnfskrk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ethpwsew.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ngvkzwyp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gfhkqflb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kzbrlqke.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3niitzalh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nybolduq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3htvrgoom.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lfcoiivb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yjdtlmqb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hwrwmjjf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nyexsntl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jlscvhkq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hvfqxjnz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rpjxepeg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qutirpvy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zvnmhpxy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qixvdkmw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ozxklnvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctmnqtos.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qyntkjna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzzlrkwi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3fazwfgib.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3znixmqyz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dyrdlngw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3goafinow.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxhwjok.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3odjnfptk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rgdijxer.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgifjsnj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3quoyhbmr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vhfhevde.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ixgxbdnx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3oxjyqmfp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pajukvut.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glmpchda.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ytngvpzt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3oqgrjwfz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbbebpv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dknbrmqw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3renqbaqk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3othwigub.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3byvqdecl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kxqcxniq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dqbonbkd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tyvikrjl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtnleml.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ymigoqub.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dwcuftvl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ojjwnnds.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jxblbxeg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3syamcang.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bmjwupwj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cfsuzfgo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xkdaexum.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3akteykbx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjyvkvo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dxlsveva.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xtpuaekh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lsbktkwj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mosrtbqg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhstrstk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvavnwkb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3poscynra.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cbbswhqx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkuasmez.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjzpprcq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zhnuqhxy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjsartlc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oqbuqyld.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkldhwpp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rntmornl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iqgmpcga.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdkcgytc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqujxrvd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfxjvaqw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ykikfwhd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oekdyryg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3setvkdlq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fmmbnmry.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wuvyepjy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wphpaiza.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3atlkgpdi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jzykbkaw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ooyuvpfv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3upwdtpmy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3whodnowc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3steczryt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mzcfgsai.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ixeaaidp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rutvradi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ifecuwyt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3flhmnlib.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ustldqpa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sqcourbc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdvkzstu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3srtadhnl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fwosxiit.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gyhwydfk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nyglgiru.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pzifajod.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdpeogjm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mrshbzqm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jwjlaqte.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrsywdts.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkbutwlq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjanxmov.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzrcvzvx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hufftrzc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktzlrgqp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgwbqtwa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkpyllcw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3riecmtct.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmgpscjl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3clrszlfd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztfklhpx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxodpzmm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3akcuilxk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pxkdwxxi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wiamxncj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ijzskncc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xdhinxgb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ylyoprmm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hshhqlno.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nittfxvf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pmmvaxbo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3nsfkqljh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yogikzsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uwtpczvx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tpxrguqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3limudzip.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wsupdbov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfxahhzj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lnxeekhn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tbjhymox.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bbwtypcq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzyfpfve.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gqwvshys.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vguajdky.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3cbxcynth.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dtwahsnq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpsmtgtn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gogpkfda.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3blkrhcrd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3auemhmnr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dahcqjrl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jebbkxvm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jaiklehp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3goqrpsod.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3omvdtsan.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzfzxhcb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3odldvfey.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gdwpcirg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ncwovtvk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tfyotusb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vrqamglv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cvuiqnln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mnqdfwrv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xbdwritc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zprowahq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nfuikean.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3drtrskjl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xqiilsbd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cksdpgpy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgdttyuk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxxfeiuy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zofgenwt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfsvthqk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3onhueach.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dmlhzwwq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3grenlbtr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fxnotulu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruokssxj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3admqqwjm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tmdhrcay.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tjelstjp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrvbpacp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3awcbepeo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wmziktio.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vldthtxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ndpdtued.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rlrpyybp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3npfsdjre.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbfkqmxo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zijhmjqq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lchlbemu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3khyyuzdx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3feajiglm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yiyjvktc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gxpdqqss.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rnbtwosc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3flxephry.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fnhufrbw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3loqdjqtp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3eetrdjgx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3umlyqnbt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mvhsechl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fpspsirr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wtqmejsi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gornqzwk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tgsvmcnw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sswzasfw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3klrqkama.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qgjgezxy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nrsqsdso.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vnppibvs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3murnexwx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3textozdi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tqbmqwhj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cxcmkbeq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lyujmuje.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ztbszhmm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sverbjkm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmoottcc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gfdlijra.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qrkvqeol.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3naowdvaa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3goakpgwm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fkihkdor.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jlkwqyyz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3swgfywil.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pwzybjlv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hirgsyfl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3txpqbubk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3eatgtlcz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jaauaefd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3myuvpvqp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjteogu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbenheye.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdtlfki.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qevtdzrv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kjizlfmi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vxststsi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sjbobtci.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wgybbukt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnbfltwc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hublbhut.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3evogftoq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fyhixdzf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ospngeck.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oobnjdeu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eofnnyvz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgaupxb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3patlazdg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3alnlukqc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zelaajav.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mwlorqzi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ecmwqihr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bbzqzhjo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uviuvlpr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zheafcrz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lzspnikw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gqjonkjt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3onyyvloh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mkblncnn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wljdigro.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bknjorww.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rldaokez.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3izyqvtwx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3feehznvb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zpqkaxwu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbacuxau.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lpigpgpk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3szmatdrb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qvvttoer.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ssitfwdo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tqzgnjyb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wlzlmuvw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3thcsbwnm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qxescvrj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hirkfcdy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rzqnypmm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gyrcwywa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3oyahmibl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3trflklas.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mnraekyo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tcfchhju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkfoheye.html


<!-- 参考信息 -->