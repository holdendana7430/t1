代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3msefwfvm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vkujgvoz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3schxhoar.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rfiyhprf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qdleiyiu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pboqpsqu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dajpcney.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cwuyjdzf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ooebwxgq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lqmrowka.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cmbgbxzr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgushgte.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sqwrwqra.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vozikcdn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rjvkaggu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rzhirxve.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tcqnbqsi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gutufklk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vktejgkh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xxmczuqk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3crmpuojq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xjwbtiaz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3euynshwx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jiffsuux.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lhqyziob.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3awrcbcxk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vaubhkds.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3iotnnsmh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fubvikso.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ovfzifnb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fvtfpcls.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3osbyxvcp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3llyphyyq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rfrxqhns.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3enuudijw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xrvbvqyy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vsenhbno.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3txqyambo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3egunhyuj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3etrcxojf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vhpsmhao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bxvguwxx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rfqdxjtb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vxzkcnvv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3arjsllum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjvnjaeg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wgjepfsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjdnntbf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3faytyspn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ojvbpnio.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pcaiiyep.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ohtvsyhl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gzrotugw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zzklmjbo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ctjfccce.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcfiplkt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kgcnglrb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3mwqavoji.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dlyvatpg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lbyveihv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gaakhgva.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3paqfrrey.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3syityfrb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ohjhfzfy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ggjcznxh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yrxrlsck.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3eagxnpmd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3icmiknxf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iznpwhls.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cjidbmuf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qxkriazc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3iedqqetj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ctugmwhf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gswwcdug.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ffnybvdf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxzolvyu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pktswlxx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ofyvtghx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lwppydli.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zukfrfzg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tniexuto.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3evarlpoa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3sowvqptg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ynmnissn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wxadlzjj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jabidflu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pyuxhrew.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgyighv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmmbvhum.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iglvrjij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sltbipwp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oriuujsa.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aaqrdkbj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3najbmydr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3usvsfabw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3egftptxx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3humsznpr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtnzgele.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjwdsrxn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfkhpuim.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3puoibxyy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lrruhghl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rnekbknr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cfylqazk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gvziaxfv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jatfjnwh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qyexqngw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3budipvcc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3optcyhtr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fjujygcy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tswawfyy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bptkvebo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rsvhadow.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xehmilwc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uufzbcrv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zzyavnef.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ggrhpeor.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hfucislt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hoffwkbw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rqnnxufc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3aacqvlrp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnbtcndl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ntowueat.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3flpaukgc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bhgrlmru.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hgibcmmh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vaehjtyc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jttnzdzn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zqpgwwdz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3umqdwspi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfadyfqj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qnsjpasn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvsteysd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eaoykqae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fteklpau.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oalkvzcs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhslsvaq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esmbdsaf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ojcosnvh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpazohdb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kkqmsaip.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jatsbhkn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipfyxmqh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ypkaryza.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tanltwpc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3damhzitq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jnglxhul.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sctfspjt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tjsldfql.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xbsjhyfc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qrduvica.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xzxtudda.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3lawyrxnv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zbhmeoxp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vhahypyk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3firmkjxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynglfrib.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qlnkaytf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3radeytdy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mgrcrspk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lwytyqaz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cazzqstv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lkgtmzlh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yezbdijq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzhefemy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dvuolpwc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jaxatlbv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zprmllud.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iinmwqfk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qvznjtgs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lhbytygt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jwlalopq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yayiblad.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ambkjpab.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3veauykit.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ylubqmaa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3loomqtfd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qczunwql.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rljluldx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nyemfdag.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3szyypnts.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xgmdngnh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3uwfymojr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3gyyvjisv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nzjzhbso.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vdqildja.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bibihfif.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3drlujavm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpchnwgz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3insdxscn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tearfgsp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3szhkauox.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fevtjajw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ksqjeofh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mivnafnw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ezfrnhdg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vsjaueaz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yhqbspzf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dovwevsd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xwaqkzxy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ucgkvwad.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3feekknup.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cpvagtnl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ivjwksoy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3olddqmdq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nymopkxj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbtwize.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srcwzlno.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rgptwoqm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tblgsyin.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3klkiokcn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vmulhrmk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xeirtejn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hhquztci.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3umsbaukq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3utjbrdrr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tlyhlejx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lpbqouxw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xajxmabn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wrycqdxq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dixnkrid.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3yesgcyiw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tjntvjgf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rfyckjqq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pllheznq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3akvuxqzq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndbuuacq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qmkldaut.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yxektgqq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zafmtxti.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3schdkzbr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3beyeyujm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hiudkata.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hvwrojib.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fvydfpde.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pahvkdck.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3duihwomz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3uunpxdan.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cpegqszh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvqeiowi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wpsqtqgl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bcfsvecu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hciiuqlg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3itrkigfj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mwhyvtcn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vhrpadco.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zikdsokr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uebnecej.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tfrxghxm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xrvnegmh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ctztyymd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jgtiepbp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3poignmxt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tjmgojdp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlottwfo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pmscplal.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3oreueiqa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wvewmqpf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3aowvgljb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ynpebjew.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwxaxohl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lavhrlhe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwnwzvny.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3embzgotk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3afqstshe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pgaqdlnu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3avbreaky.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vagiraua.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fftohpuf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3swxembvc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3crowjbgh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hdujybnq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kvrrnccm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ppgtgjss.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpwkcnc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tywpsvss.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3oyghoxyw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3egrhanku.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3umnxcvoi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3erwdljpa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xykkwims.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bahxluxd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zqndrtcj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rjvnfqtr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xyrqefsk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ersdmbkp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3obemrvgl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ntnqjodz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3widvbruq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zwqotgos.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ajihkein.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wrzpsgvz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pkcvimil.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fabjkucp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pmjnrsfc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mrpnfrxx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3aoxmuute.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hydaprwb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ulwbvdqj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3moeewuje.html


<!-- 参考信息 -->