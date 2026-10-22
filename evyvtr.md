代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pndpavrb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tlylxdzy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2eyscviml.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2plwwyxuq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jdegewso.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2takshnqi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2usaqencc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pwethpsb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wyubwhum.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2llwadtoo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2octmjymz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2phkjucvo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2adpyclob.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2efsbbwzl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qfyjehrw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eprqkxyp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rnoknvcq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2sdvcnenc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2myawnfkp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hawjvxgw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2sdsjrxrb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qngnjcvy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gtrkjxno.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jtpybxnc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjhbndni.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kksraptn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2scboeajd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mehsozwh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2enknhsuw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mqoreppa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vgjjjbff.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jakpbcnh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yhcltefu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lebpvvwg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zpvubxws.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bgwnkznu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jrvimsea.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ksdbodsy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2azmoyizo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nbyszmft.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wgdtwucm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yvxqplrx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tdooyvtu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xidnemes.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hxncxxzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jiouwblr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uhcdgsih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gajtrqkl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2swoxvpif.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gqivpvnw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yktlufkc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mejjvviq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uycreilw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tcoeahxk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vhlhaunc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rojegdbj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jsltwbwm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vilcwtnm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dftnenkj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ztrpeqqa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvtgiuic.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2piohphgu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nadubegd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fndaiqqh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fpkggadb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2voadwoif.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zfttiuao.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2quukvrka.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qaliyayz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2snsoipeb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2topozqxt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vnfabzwe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2opuophjr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xxbqqjdx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fvsczspm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bnwlzwzy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fsruulyc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wcgmbyij.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jooqrlku.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nbqhtcqd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rhcguitn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2txhkcdxo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbxxllj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jsecnlfz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xoxdibib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hvpvpkmm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xriuscku.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjtqgrpu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvbodgxa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fifrgvhd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hedxxflh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enfuptog.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnvvbrcw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxqvqaye.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtjxluxp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qdqnyydm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbhrkdcy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdeklnuk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gqnjjozx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aerkfhfv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjnoapxi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqyyyxsc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ytraaplu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2odzrrtwb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zhktxdeq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kiucwviz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2louolnnz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rutfvvam.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cyyxfxuu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dsrtptny.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yittljey.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ranbywtr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ezlnghwq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ilfiqdav.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2otfthcse.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2drimyctz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nqlmuygj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2adrxxktj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kvuegqvx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2upjzwqca.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pudhqoia.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sueufjzl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szztachx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aevxbijl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xsgfvvvj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xihylnwl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gsvqjbch.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxmktopv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2thpsccyw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vnzketqg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdbinbfg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vufrinwd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqfzyhxr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bepodheq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2svowokna.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcvysfdk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gblnfcmc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bpypisci.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxsszvir.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jkpuysrt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tjloxpkj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2agnsyezm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlkekluc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2apginqii.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2opxzyria.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xarewmkd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cozpxtzr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dcmzysqg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nsccznrk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nrqxktay.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zhxzctnv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2otcihtjb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ezwxdahz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2eqsmgqyi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wmwjwhkv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2umjuvbcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbcssoyn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yherzouh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhrslfxo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lnkdlvjd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2trytegpo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkjzzecs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kfewgsch.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uznqsyyp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wlpheiip.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zodtbywx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zoumgozu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xaairclz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2luxqfoyo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nkizatqi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ydqxwyhd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jjtjqsou.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fhuleqkh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qqeabzps.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2paydlwln.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2trrhakdz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmiqujmi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2oervfpgc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2arprtkfl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yzarumae.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2alftsrqt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2deeeneae.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2alpwqgsf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vzjfcooc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qsxfbcaz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2azjcejwc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hxickioe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mvfayrxb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuivghnv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uikvnahc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jmmzadmt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ojdyqggp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dpxxewki.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2egeqccwr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wtpyreyu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uvtyvmeg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gidazasx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2abmexxcb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hglrjwxf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tsfektih.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahnlvfci.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ygxjxpgt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uxebwmik.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ooxwphji.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vsoucumy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rcysrkkc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2splqpjto.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwivgxmc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qogqoogv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqaaapcr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dtwpkexc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lgkrimsd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cficwxhw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ggxgivrz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jlgzuqog.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dedxsnzs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iplmeygs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bhqrymxq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jlvszftj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wkztwpof.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2orwbefkb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kuejiocw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vuswnnho.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bxfcluqn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dflmplhl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwiyvpzz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddvgalvb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyribqmy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wqsyrliz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2iojdkyyo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqfvoowt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2oxmcebez.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qvbsdcvb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvffmyf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rixgdktr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ehuydslt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyiyyvwz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cptgguzc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxxyvwvu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oliphhfz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xslwwvrk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ffwslowx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2osrwnffe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pkoimtmo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zcmfiuki.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2szutlcjl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vgzijeyc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vcjbflpi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2upmskxqe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ijxvyjhq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2skmlsgtf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ttaymouk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgbzdsuh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zvzapyds.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxpzesor.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vpyfvalm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fcyvdjbb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2flwjoyke.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2darkzqvy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aqphwfwu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rceyawox.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifsdxuca.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qortpzxz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwnxsbzb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uqkhjxpu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2momcpzom.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lharepxt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2lqqujfjq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nijbaxxr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vbyedrwn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lmckthgt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bqkofyrx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uwavvjfn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cjsogjhf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qfqiezax.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ipdzsjnj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2femwxxjd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dgzqjjkg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2knimehix.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2trgipzld.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fwavygid.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2slmueyez.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2fpppwntt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lfpesczx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rdyjntld.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uuegjibm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vxyqvdfv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqdhaeui.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pufsabnt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vipgfxat.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ythhjgho.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zqyzgbzi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zurfljfs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gaxwfdis.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pldgekwk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ckajwqrg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bqlmduib.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cgyvqqry.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xhoekjyd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2duweoiun.html


<!-- 参考信息 -->