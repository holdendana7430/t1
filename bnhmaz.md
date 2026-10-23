代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ztlkakek.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3llwhuxzt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ylxsmuhh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zjaptvnu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3szaiwbvk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kijujecl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dibxport.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hwfodqfa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3emaibhbp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ldhmwbnc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tfroimaq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bkibacyq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dcbwjkso.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rocboknf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxkeyoaj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppeikexh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrsbwgsb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3sygckgto.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oowkruzp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3elipwcdj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cyridqfv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cfxuszqk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ezdgemsh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bcczxpvo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nsbmswqm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3yhoahcha.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tcpkaksx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3arcegfnq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jiuqgvsf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tcrhqpvv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rayzsxqs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rdgjlvlm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wfxyqgxa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3raqxnddk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3moowxdlb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rfcjmyoz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ailmdvva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkifbrlg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3eochtqky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3juqzisdr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3eazcmrdk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wdhkkhmw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hqorogiv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3owuqpsaw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ycjuhodc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lkoblvat.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3bvwkdctk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcyeczph.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkpxqhzw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3iztyhnyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3piotsagk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3afreptik.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvpztbhf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enomcdld.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3phoelthj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ozajrlnd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3pdtxuqpj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zayvuvqj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zukostgb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hnfgmezx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cggnrkit.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3czryiurn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3njduaejn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vcimxpqv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ehjkbuzn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jvvwgccb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xthrxctr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfvvjnxj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dwstfeli.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3eslxatdn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rtwfjkle.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kaiaandm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ydimlpiw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ewzdnwof.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dvoewybz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ydsltpol.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3subymuzy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3oxienucx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ftdrhumk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctjqorjl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qajalpij.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xulhgtkh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3odvlrlvg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oabnewao.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpcpqmck.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fuogavzi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eoijnupz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xkdpamvx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkwhcawe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cebjirgp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ufxcgnfl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbrwedab.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctseuvxo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xexpzzfk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nilaoygw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lhzvyakf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rjimlfsq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mwkuuugo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nkvmxnzv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yqjqmsga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3beirhfpk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fqaidmqt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hwrweguz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lysqlycl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qoagxbgv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvahqfkp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lmmynlqp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wklbcyjw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cuevxyuy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mrwtrdqk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fnpwotdy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nvnizecq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dbrwasaq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3smeycnuz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmsklmhi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3htnrzwue.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3isfjivil.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xyszzvki.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3iuvsaesg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzobzvum.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3spkpperw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jrakhehk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrovekgf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kkhkcjmn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igppllsm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjotlqhn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ccqcpxzj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iuinbzzu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjodxdep.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtuixlar.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fmiwagwr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iuqdxdrk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3skkfyzjs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sophdret.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tindyyax.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbehina.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eqinseuk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixiighaf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wepfopvv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xutgiyll.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ftrzactr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gjjfbqla.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qvyxsavw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3niyjoxkr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jwpkyenf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yosesxbu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gcpaeiaz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wlpprbrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfnyhzxg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hssxyrpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grvczbou.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bhcooxml.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ucuzwnqu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3scwbsuyk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yobskend.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbrrrkir.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3glcooedj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xhrvtpcs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zdjhcwyb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3takfgoyr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cfiouxqf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jvnmurdp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dykznhct.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbpwiejd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qdfsxdgv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxktkgio.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3sivnlqcm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cdftlygf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgxonrxi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fdwtscvh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gubogyrf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3larzpjzt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yzjnhxvq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hgdytvaj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dzbknpyy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3veyzpxkh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aveqdxks.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fjowjsky.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gqslotaw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3htcammiy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brfkelmn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cdwagsgv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yeirllsb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiedavuk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ksydfjdx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uqfjfkhv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3agfapszx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cqknbopv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xvhhlosi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lqssirpm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qthuybtk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eitweaxi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sybxuxfy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3cruflsru.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wofqrxjn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mzlrfigz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3clzriitn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3dqwedrwl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oqogupxd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ckpalwsf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3afcbhtbb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cwcfrypj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kgmowvfz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mupqlnrc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tcikikhq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dxwxerkl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3afdmjkhf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ldhyzedj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3plwtmago.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3meorspxi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ubfxddpi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kfcohazd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3naecemrn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yzephphu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xusxrurj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3plifisfn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3etpnnwar.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xanmqvre.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3eofzjzxo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckpnulkd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wdcahtoq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lxlgnrfo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ggjyuekj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zaqprcyf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ffctxdhg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdckjfry.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3icdkrmbg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ydedghhh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zgfuxqjb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jmfmreif.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ciuuxhuj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tqyvybkx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xfvclgok.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fiqwajjp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wezwjpba.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xonjkdkc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pmkjqfba.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jcxoirxf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lcgfpvpd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hhhxgexo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3eezwyrnc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jumljrhl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ocoggyrc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lksuuxrg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubxgnewy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fncdenay.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yuusrcfm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jbphhzat.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xtfvsczc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcezpmms.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wjsalugs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gegpqkwc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zfgpzwok.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3imkmbnim.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mfsukyam.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bfqaiyay.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bcltuupu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wvopcyaa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ajjqhclp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3babjvyrn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qwmhdons.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fhyrbldl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tausmeks.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3udfxmork.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3befdfggy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uihmeeng.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3aezfgayi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3cvezsepg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3veajgnms.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ixzlykcd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nkbntkmt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jcakttaz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wvnqticp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkrnttko.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rnhuplgx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oafwlldm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bstarxml.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3niinmirt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfudyfgm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jxrbixyk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jhxctnnq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqlvtkls.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rksmxpot.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ettvgbtt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xrcdwrbn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vdguwobq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3aduzrdax.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rcxaylaq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ehuaxqyp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wobgfdsm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vxfyetsu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pmvbtuvb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ldgzmsbl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qcqevclo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ehanflxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vowfpmcs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ilxbslem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lturhimn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ldbynshu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zhyanusk.html


<!-- 参考信息 -->