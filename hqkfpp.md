代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tltihelc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zovpagud.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oygfdyyx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mulhujvg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxarrjv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyxxaqf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jmxaswqy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zjxxdbsz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3urgoftzg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3igopqvxo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3evqqshnn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hzkmrxaf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kecahbcl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xlwgqwkq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3eeojvubz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jybnvewu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3azpeyyog.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dklgkvww.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3voobxxvb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rdnvednu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3knlrdnna.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scddxtck.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pujbgzvm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3moqhkhlg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3reyppjwi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xkpvcefh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3cywtsluh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3angnqwqv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bzizpqxn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cxkkgahb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qqmcgbyb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3idjaexhx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ftpwhcyw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3sdpawwkr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vymfsjub.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3erqylplq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dyzoqkkw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfxioxpp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3spqhmxdt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3upgsslyk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aefunzgl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fhmvwfzm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fambsgcy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hmwujmha.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ahsbtkjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpygdowd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jwwruxsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjayrhpn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kdwodrst.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cxysnfau.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3igowrldj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vvxkskab.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ezeagfee.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3trrvhnsm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3akwpvnzn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdeefhlw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qbiriebb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fpjlaytg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mxlupuhv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3nflemptc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rwpzguxz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwjktkms.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xtlhbbmk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3glykffjz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bqfqhegm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ggrmjadw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zlndkspe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3koxvbjkw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mjjbhkmp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jgeobnen.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nerhmkye.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vejqrxwo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xecogdfa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3csvhducx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uwxfqlkw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3akgwsfdi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ygiaakkz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pftpjoom.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lkrusczo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qfepchzo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3sbhyzmtl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3diyhmasy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhwrzils.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zymakcxk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fhmrzqzy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hdxlhmjq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oukbvaiu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3deixbegr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqmspbtw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnplgzkq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3yppmnytf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzbeomsm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxfkgclt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qugyqdyz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flxjcxji.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tgreyzmf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fibzowwu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvmqndi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bbvubhgr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frjuuxkr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3diqnnnek.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijouyzmv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3itxxcgms.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jaoshgcd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3alfxqxtc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tkmjtlhu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iqlxqhuc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wgigtutg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bmkomukw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jdgermmr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xbycojif.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3pxtwzpfi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mvployus.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3srwfeour.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jsjoavpv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oswbbprm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kbcjiwvf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gkwyovrk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fzfqxoyh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pdamiild.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rgipvvdv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckjajeqv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mqpiazlv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tiouxuyb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cywmcaxb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3opbpuirl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3phkvelhk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgloaerq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3egychhrj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hgucooos.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uecxmrcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lqcfjmkm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdiyjkqx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdojdfto.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bamthxwq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvgwyfmg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yznyofgh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utxcpwbz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dtkifkfx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zyxzvogg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3epwlnzds.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swnngngc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozefgdjl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwacumh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3kdqegwcd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymejgque.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hiansusp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3uhmjrbuu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wsyxujyn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qocbbzfy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fbxndtgl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fvqdvvkj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hugsrclk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bqtseasq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qwjxwozs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ciqnigdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klqdssxw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3iiciaoyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zksxtxzn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ocqbcrzx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hgjlnhpb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqyalphf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3haisfikp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nebcbifh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vfwexmsf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gqmepbrx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3eqvfypis.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdrymfof.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ysvoxvxh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3dkswscrh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvejeilw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pcrillfe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyngtbbo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mwfsnlxr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mskwxqzx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xyvscwuk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mcpibjlt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vfpzgblw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fdbixqtg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uhccmyjk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kxopkabj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rkkyfpvm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iedazuac.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wkkzwkfj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zwvefaxq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vtvurvwk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dciosyhc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qqgoxsnr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obeookhh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lekrtosm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayuavmsr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3shfkpsdo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sjnvajdh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmghnihm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rgxtuqoh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xhlftosg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nxizagob.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdzfmadq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ucnypifo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3telogqgo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyrcblqu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3oyvccmap.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgjgvwsf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujdsfopy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3giuccfai.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3embdlbta.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bcuypgmm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rfkdeyna.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nujzzxjw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3isrtkbtv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lyimyzpc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3eiymmncc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jxpluwfb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fopmjsfb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dishstkg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vabuzpde.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vggummpv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3papccdgi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zlcwpenu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ehicubdu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bfyppxgv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oeuyqdao.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xidjscdl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3iksymcha.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pidxyimv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vmwabgwp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ublqwdhn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ogirzqst.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xtgfesjd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3encghpng.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zvfllmwi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nybbidkf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wkyivhxv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rykweoap.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3idqtpzpa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzhtewfa.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbybgtrm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdobtre.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wqmzjglx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pugvyuvq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nlgxsqtd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qaumtwju.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dwlllqio.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pcxjcwbe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3djyvcglo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jonzxckr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3znfnmvkt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kiefmlgg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tlnpicyf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3slkremsl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zsfckttb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pxtotwfb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dnguoltk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3byfjesfx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxivxnmw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dgudgknn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ndvkzldr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvojorzt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dovpzror.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dgoxwjvn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhspffzk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fdegmpod.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spigwzra.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkbfwitz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3swwwnwmv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jlamvnya.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3onqwkoug.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkpzajxx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jsmyivpr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xtrsxkhf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rzhxjdqc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xaqwkmaa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zohwrunk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jqksatjd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3smbcvhce.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cyznstdg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3tdwwvyij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pspkheou.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ezggjapz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cyqgnjnl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wdmfkylp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eidvlmwv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ysqxbmsm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ejpkzirl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hkaiorfb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ekyeegfz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdvprvur.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3obiycicq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3emmanjzl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lolsyjfi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vrysdfix.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jrlmsfxx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3myyhrtsm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfszerpc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vysycbia.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lkfenpmq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pfefdisy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wsmalbqy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3omqgocbj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nnslsbyc.html


<!-- 参考信息 -->