代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zgdewuhw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qxikzrnr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nlakqrfl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dfcgoqzh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xynirfty.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rrjypabv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xpexjrrw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3twhpsqym.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmnbual.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qxnkuchk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fexbvhmm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ckwwlxgn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pmuigjzf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gutelelq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gobyalol.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xskjiyho.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gbdwhkqe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3nogvqfmm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mxjmsisu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vjxvkjcy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3spxzreco.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dwytnnra.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kxxmvffb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zlndaies.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3omjoxruy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3otwxrkiz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dnjncncc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wzxhlebr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3prtfinst.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gbxmjcgz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ulkjppmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tqjwwovr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3errsaell.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3olzkwcyn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xznocgpy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rbbxisiv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hrarqozg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tkcmvrto.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3axxtkuir.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xvdzryen.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uryrgeqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbwbqyxm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bvxnztla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxrnkyfk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yhxadnfv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fpzvpeuk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vhsigqfj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mzjdwege.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqtkcqx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3liwsjahu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wogutvfb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3muyianqe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azteecbr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xlfkrdyh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ribgedqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoydgalw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgkeajkd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwxjhynw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qfqviqxn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kgvhtfjo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxuwnec.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzbdcdot.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tmluadoh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3adeovpgg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jiytdqvn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ldludwvm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ltnwmftk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uoosqbub.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ooulosgh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uedlbvjs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ywqlywvc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qguwryvo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jaygangx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fjojcyuv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tjharwxg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kebdkfaf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3optywrcy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ardjvffi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3luvdbmqm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3bpngendt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pwubiwzc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ynhxyhtz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vgxdhwxq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iadvmfwn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3srvgzolj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iliuuray.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rwygfuvf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ryjvbtra.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uaybdomi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tmpqtsns.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbvbvcqr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oeeronbo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zeayngrs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3endruyis.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ajfbiqtx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ysftysct.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvrwlvmr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vwltaurw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fkyuwyvl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3duoxiwje.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iandoupm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zpemdgia.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cvpykqyi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hllwbzge.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3yyoxshop.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3czpsupgv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jmamalee.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bnoflcpo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tsmezaqi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrjkqftu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3doqkinhi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jazwpxek.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vbkudloi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3arremwmj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xnxnlahm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rwxreuxk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3serqzuoi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpfussiw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gajrmlpw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vpnhhpkj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3icpyhtzx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzlxgtxh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gwzreqvc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwdnprhw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fnxkodvy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wtsqolgl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvssxumw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kprkdcfp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxlcbrzc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpoyythg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vlvbxdnh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hokerkmt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lasljccg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlwejajv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qzafjary.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mokjlmks.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jiwwxzrf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gorsbxvh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cydasbgb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3exkjbcpj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pgfpygct.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjvsyidf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3efboyljo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3htqkijkx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3orgxxjid.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zgpbndcm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3juycgqac.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fqlxtdzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3orzcfelz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jtogacws.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vrlbtdqa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uclcwqab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtqmvblc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ndrvyhad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqbabwxo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3eubamish.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gvpssfpb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zigzzboa.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3povkcxmg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xrkongxe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iksasqxn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fflzaeyz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nbokmonr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rrxxlakl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cisxlhmp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3sfwnyjvd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jwgwsdhl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ccvinqzo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3alcwnrle.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgcglwdg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3emutgwzn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lexulvfu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ljyjynyk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3uouxfrwm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3siwcgnxr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kymbobut.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xgfkrmdm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mzoffxct.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dmeaexan.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yugxdais.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3twuemdkn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gqhmxrjo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ahwgflal.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cqoyhmto.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3csogqwds.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utdfzbev.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztefllov.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fozbovdr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3chtervzy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yejldwvg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zcmhepgg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xytwpfbl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uyqbawql.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufuxriio.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmglzswi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hnejqnmm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtaxqihm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mzwapavm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3sqdgziix.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkcbxkln.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3axjhtgzl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lbfggssy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3knlsvamk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3avtgrgmj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvolakfy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3edfvyuyv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fivokvkb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlynvgir.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3osqnaafh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jzrkbfsb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yhxjfloq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3upnvmrqg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdlbsahq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gikhuwcb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3biwdgfxn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uqnlpiza.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dhzxebdi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nfiawmlj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qpipqcia.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vjkescym.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gbdrzduf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mspewebb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bbhnemqx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3apukmknv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mdhpxamc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3prctzqei.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfbylxah.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3irgynmvk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jvsqxnwo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyukutrz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3peiorcmt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dhexvuxy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xwglxruk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hrgbnovm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ybmamljw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxzplrhg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3thpbqadu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3kmkzclth.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yhtuvxdy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3llvvubmr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vpzxlymg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mwydclkx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3moklvbfb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ebzspnwj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cclkmhkl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hnxspxhm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dykcrfan.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qblkfcip.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nnytazoj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwjjkwes.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tjkwjdya.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bepswyee.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wjziqmxd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3oglxyalc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bijpatyi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ejozeamk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ohlbtccg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3suobewov.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekoahxuu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zaonfoxt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3brxseyqo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zucsrojs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gmtlqxio.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nqfocfnq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3krcelexd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rytbhqye.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tamkhmeg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3adetarpa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ntbpzgbe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jkvfjwxh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3iozfkxfh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qaytlzji.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rhosljjo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vhmxewki.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kklzaxeu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3eybcdvak.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jcpgvhav.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3coddzqko.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kpftcgvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mtzmeyim.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mxizykpn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lmhqmxlp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jmclxmbr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzcchgjv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fhlativb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nqvnwnpb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rssqkiox.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xrpsnnqj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3tdednxme.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lfxafgxv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3aknomamb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kvyidycx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3etoixhpg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ohvwggcc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ahrdkstk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bmctbhgb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ghmsypmq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qzrkodcj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ufizmofd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ochmuzti.html


<!-- 参考信息 -->