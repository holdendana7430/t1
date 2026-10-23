代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3tphgcsbz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3czahsagj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3stzigktn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ewcitcho.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjdgqii.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nydgsmrz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uxkpfhua.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zavrjiqm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3julssjpe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tvnzzajh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ltvfghni.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wpjjufqo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wfobkewa.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pdftkrla.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3sruvietl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wzfgiyjo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3uidzbeuq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3afmauyno.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3aeunxdon.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3aicmhoyf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ezplheav.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3emdzpxna.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsbwxrnz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cyrunlar.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qnxowdal.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ucccmjss.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3okodsdxg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3emtjjvgc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3auuvjess.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bzeahmto.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mjavzwzk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3copsnhdz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ypsdnpme.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uenijies.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sghmhlmc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lnowmhrn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lezsotuw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kaegzarl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ypiweagu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uwmbxbux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xggtzgej.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pbqonajj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gkpiybjk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rmgjmees.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ncnjfzsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eipcecvg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3losybrhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eywnqozq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vuqlpeam.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mwjdcval.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3evxortkz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kigiedjd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gupjpqmv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jnuimzea.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3mjihzkgt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfucpspi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3popyqyed.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugvjauum.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uqjfiglz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dphjuypa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tfoaxvgm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vgmqgjaq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uicatlyd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3iajdgcgf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dlniyzyf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrvemyzw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gghehisw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rykcwfaz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3eorqwgqk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zqxsyfjx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3srhdpseu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oblovixj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ushlcgdf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sdcfaswl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ijodgvrq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kvxbgffc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gidczakj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nkzdpdot.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kaqkgbqd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kaitnvgf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lscekldm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tcqzkzwg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tdddrrqx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ujrknero.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xchdjwda.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wbgdmnat.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrgiqlcf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzrvkisz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kximkxtd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jovuhdas.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3demadqex.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbomcqlc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvomewur.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tvjdowlr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdkafipo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kwwnciar.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwukjzrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3viwlvejc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3akbaqssj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcjubwol.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtewdemr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3csccwepw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sfagduct.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eyficzad.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3oyjghsao.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vrwbxbbp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ybdfqezf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hltwxpcw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nwkqeagj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dryxamzu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jxjzxvdo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vcbjofio.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lzkzulau.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hntdbkxz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mufsbgle.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pryetwer.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnlgvuv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3kmjnjzot.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nzunwozq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kyisjxrq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nbxucukq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljysbzlp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kdtzfqli.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mibxijrq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3okygcayf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yorleugj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vretbdow.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjcnjbal.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3abbnksmd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lrjdqspm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfqhqauu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbwklnhw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipeteayk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixkaqvdd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3alfgdlpa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdiwigmx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdnmjwqk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oivlwpat.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfkumyrz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzyvugeb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gyowcfkw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcgoeieh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmkgmjrv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3apfyqlqm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hzbcmwcg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uyxyrvtq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qidugrdk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qwrcfuxn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qlpyyiin.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3aenzkilt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jdefbigd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hppexwob.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3siassafk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3izwwojjy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pqglklpb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jqsyofhq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuqfiqck.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oxahppqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epwbzwjl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lablceck.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3axcpamoi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jowolyld.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3naycsmzc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjjycdvz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3odncguau.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bwrnolrr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ufckjhrg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmbgyuaw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kofqrqzk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tbyurxwn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3auscyrcc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsesklad.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3krarurka.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iybfasjg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3eqvkkcew.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3eaoltlxt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrzohvot.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yqcsfoyy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3begpjvnr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xamrwpgj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vcdsdcds.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3cbmweaga.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ezuottbt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qoowqbku.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ctrwnoko.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vxeqmubg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ydafxpye.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gadgeeby.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvowpfbr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsgozjpw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zfiqdakr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dbmsryei.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ccqahgus.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fhfvxcea.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jgrjnapl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3himnakpl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wtqlogbo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qjovwkev.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cfphizyq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vurjpvlm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuvqhixs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jytdwjqv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3njtrgelt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jewffiks.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rjeotbgg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rxnfldbb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ytjhrltm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bbkdkofp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdoihhdx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfjmwipd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wiiquukb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ckhcoqpm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yxuqswsd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zphrkggk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tnafzcpi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kkdprnhm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qoapahht.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hbrnqold.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tcfdudyn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fstoilum.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3brmqqxqm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nzinnjvr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qytygwrh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eblbrhoj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3adydalgx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xhfoxbus.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zalsibve.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vgvyxnlx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ytjznhus.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bdtxeeig.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbggxowc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zxozwnwx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3degkepdz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsuhnuqn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3regsyoie.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdleoxah.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3httvngvs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3sowtodtv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3beokcltv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjpftzon.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ptanirvt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ibwxacch.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vhzgepao.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xquaetmx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3naawnwxh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pkrtyupm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3oisukmqq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wxpqncvm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cwhfstbw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iybxxhss.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cdewmplu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxdocjqa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tdjawebz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqdygzrz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hovrkais.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3klvuoixo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ersdmqoj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pkjwyhwp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mpufabzh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hbjhdiox.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wojpkyda.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udnoavta.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhvugbyo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ebtcrdsm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wqpaxpky.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3deqyvmeg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dgjhkjyf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3satwlpmt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nalnduah.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eqikutdw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jevlpman.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3isbdygvy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dfaqgchq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vwntmzqv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qidqpyux.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mftxdjgq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zmfmikta.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tckbzzhb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vvmkgkhf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3riqunrew.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cmhojcxh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kerkrukk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zpjfcjwc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3btljqfwo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xrpmvkuq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gxudhzve.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3uswbyjes.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwvyztym.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zdxtdwdx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkmmylla.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3najpmcij.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rdkgijvk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3swygpayc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jfcbdigg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3aexffcfz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3juppcydu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zuaegskh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lienlbza.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3znybdxgt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3spmmnoit.html


<!-- 参考信息 -->