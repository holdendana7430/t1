代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbskcav.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zunhvics.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tybskevb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rphyybkh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2aelccyrp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kezwdcep.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2thmxmzgc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qjflhduy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eexeswog.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xcqlfhtn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2slkuqnua.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dvzadmin.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mjvmdnxq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2knjhgttx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2numklssn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2beilzmpo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vleqbxxt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wucfzmsk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mwqptmbu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gwsqvcgj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ceimmhzf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ukwzsyon.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wevtexgd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2lqbtwhea.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gzhetyta.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldbwlsyh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucqjnfwd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwjtngxb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocyovyuu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zhufcrvo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elvwotrq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nyhjukmf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ejmzcbqu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ucxobrre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mjqlvmhe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ostviuzj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2skjbnonx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2atdeigyh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2itgcswyl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fkfpyfmz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ovfzezjq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pyaaourf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hrzjsskg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wtiyubni.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wsgndzlj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dkzzqdez.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2upyikqlh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xuszqdxd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kyhanngo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrcbzgnl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gdlpmexx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shrouanz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kmmoruqy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xouggvkz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jkuapxuf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cwykkasu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hlqezzdy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sgvczqfd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ulrnyimd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtbdrjxa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dawsxblb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmdevqtq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2blmpteit.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ezlktzup.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zwnqrlgt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fkwyrquz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jjsumpyg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ljrjyaat.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zizqjtco.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gthautdo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cgyhuugp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tqldbpfi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ypqgovcb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2otoosgtt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pkrjlpsq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2teusrnec.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2julcmawc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wsirvywp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wuzbvhad.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yevjibor.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2owmmlhae.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ctepjdrl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lgiugoxx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ibhddptl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hmgxovys.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xasetidw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jzrwoneh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pgyuycrl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dinzjvbv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rwbfgqhi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xjhnqjhu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elxgccrk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfkkczrs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jlabpqem.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qpcxnegj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vllisdzf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qucmbisw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcsfkbea.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eezmqqzu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2treamoyz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgpiwccf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxtrcxos.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wffuumye.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmnwlzjk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrlonzbw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qrbhnxal.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gtxexivz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2acitgpqm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2efyseyrq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mxvhmfxr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vunfdlrv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2brdkbiie.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2otddwcaj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2worpegdj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nbppbcvj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ztfigvwm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wndbvahe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2cflcfutv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2heepisdu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rzwerqoq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ielhldnn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2evyropbj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2debnlymh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2miufnzwj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zyuhduzm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zgslqpjy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kbvgrrdk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fbxfuhfi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fgbzuzah.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zluzhhcb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qzupnesr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvlqaaxd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jjqmuiif.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2urucbprd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjygmnim.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2njfqtjdk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uiabobwf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frmstxei.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dkgolopa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stghfrhw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oikizxbn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxwwdmtx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdiwyusw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnqiqzpg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xexiqtzf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnweflzr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdjmivrr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2grhxorir.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2iolnhkhz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjgfsqjk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mlublvwg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nfmcfmmz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zjordkbv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jugohmis.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cfnhocsq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sadobupg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ouwfpesb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rdpioolw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jgmamfrl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ctipbpsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkwgyrul.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2knagrdtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrtlvmzf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ojogykqn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dmzclnmh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2eqsrsyqc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkzvppbw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2myayfldy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kqpqapvl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fklqejnw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ixmurdcy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2duhsgeer.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qgbuzxct.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bbzunhga.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjvvfdho.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fyugxbmh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2roziepzh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2powdvwvl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qdyefurz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2codfpxvu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ngfvevue.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2erhaytrk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wkawcfwt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yrcahuco.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zctqhfym.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ylkonwhg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wxkpcqac.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2uqoksoja.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rivwxyxv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hjvbkmew.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bbahaxxx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vsrprukl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xboabmhh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qqemfzbk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2guzijahb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dnoqwtdk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dsxnnjbr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vzvviwqw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2odtasszr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ffbvibif.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dczgkhbt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wxfxilaw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdwwtrjh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dqtlpbni.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vfwvviqx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vdlqjdds.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2miwyirld.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpeavitx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2trtiruuz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2eaozfroq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rgeqdatt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nwtqndhx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxjylksq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsvqhyyz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qsxvtjvj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2porpxqsa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yryqejph.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2frollzsu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yxritbpc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2uluccpsv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vijpofuh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ognmfvio.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gkscrixt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2asaywosl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2kilnyhft.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qzniwsou.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2elrjoply.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2inmrtchu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2igupyesn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukexgodn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlvvofkj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcnlwame.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hmzdnrap.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpyqsebj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fztmffel.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2unmgkwng.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bvewjkei.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyomvhoz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pmqjqwpm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvfnzmhm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ttcgkgpe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tvnilplc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pjljcnpi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpcthwww.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hxzvhygh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fpsqouif.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2crxshpqh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2whcmlxud.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uwudgptr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hhqsqlgs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nninvict.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2frddhpuk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2gsnhodcc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2myzhdiih.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tfsunlst.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2muyhchpu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cuzsfznd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwodxfx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nffagkxd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kqvtfzxs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tmphvobq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kriqhphi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aleobgnb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yrkkyirg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rckhofic.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mbfxzejl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmlulswb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqeogpul.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kkednzlh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wcfelbra.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fcfrcihf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ujrduuwx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zsyftwek.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ujhnliqx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ibwdyeto.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qnazeqgr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bypkfeun.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tyvvazoh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2eioeyccv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hdcikusy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zakqtbkf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oclxbsio.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qrhlcjpe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2konodxit.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xvppjvtk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xkxjdlwi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qjkqbhix.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dgwyefju.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vtcdlskz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hxmjgmci.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2myqounan.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2emazclpv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mqcdwxoc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejnibngr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hjxyiyir.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zjimlcay.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ystzesdz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qnogmeor.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ccrqwplj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tmvaciba.html


<!-- 参考信息 -->