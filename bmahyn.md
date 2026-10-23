代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkycywuf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fearsvcq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3htpkzwlj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zimvrqeq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3jutbdwey.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cgfhblgi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ylilayfl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sxpjlsdm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oemagjxk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ligvlqle.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fnrllmsx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yynwrblk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ngsovndb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hsgwiopj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hihyrefs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gcfxnvfx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gwkprtwi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ztsjwyht.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ysdgpkmb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jraskwoq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ifjuezhg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3twgphvnc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ljynkwoz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mptsmkpx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dktxsbue.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jurmznfl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gptaqqtb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvcuvjhk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqtzfypg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mzqjzlxs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qenizrwe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vmmdihtu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zjpkcwuz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bqbmqydh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vjbjuydm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ufbrrjhe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kpvgrowf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3uvttnmae.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oofdphuy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hixekcxx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kdvsasot.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fxtjfism.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zpturlio.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3feynmtpe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uvrjmqjg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jihjdxfo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xijntswu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjqetuia.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3amewxhbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmbsgifg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ozvwqkfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3catngazf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nfcbbefc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gwnotpvs.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ufqrdwbn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bodhtptb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3khnqpmso.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3spwgbyzn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tmtfyfag.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkotyonp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hhpivsjp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3inotjwzn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3grkwsnnc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqmpmmbc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jgkxxzet.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrqcqfhg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rmekruii.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbfaobtc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxoinom.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3twzpjbvx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wxmfmvcs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dvrczmpk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3joavabrd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pwncboah.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wsyxeabj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3npbssthc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrikzbu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cforhtke.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3frdpmwex.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3extjnyhl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mtwmuxkb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rtipgixp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vjeqdjje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fyfooban.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xaxdbczj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jziwoymo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3oduyzlow.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yhraposw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dtlwonxv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pjsfflws.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qagjimit.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrbgommy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okboohnp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3faoawkbz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jsjqjxdb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkwhiwdv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sfiajhkl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsozpkhb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbtecyvq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bydrptbx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikyzqvms.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzbmmmrb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wdbqcqps.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqnxhucz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3boafstpv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3azexfzwh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tavsgqpg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mkwupmfw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fznohxka.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lbkmkegr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cmvhjnvm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jmqghpug.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kktkuczm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wcxftjfg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3scmaztkd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3icgdniiv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rckbmars.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3smxhoayv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bzqnutob.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ueucrgxw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zxpgjars.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bsmwbdwp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xvxpqgas.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pnllydcu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rzeynpbu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eryaxzwh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nrmvywvl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nxctcfqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dxosnfty.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ncoruyjg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3skxkmtde.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kokibvbe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mnrnetig.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3udbupbdc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqyomglv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3osalogwh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbdqiiej.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncgpcfbc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jjstczro.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ropxrjpf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wikeshuf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnusmkqk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gerubspo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnyhbcno.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3abkeavfw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mewpczzl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukzktjym.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wznxlxxa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ijvohpsj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjbkwqeg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3neuhueua.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ugxcwiul.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3unxzyzyn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cbwiotqp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kvhxwksz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lsltbgsu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cviudgwa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3badnlhwa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bxtutknz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yajqyjoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keduqufz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cvhcoojp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxfoprli.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uhbadcxw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dmxkbrom.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dgxatnsi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kbqkuthc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pxhebako.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gpdhdwxe.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qzdzxkeh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yugjuxmt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnepbose.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bwzrzzji.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hiczsfto.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3viiqkrww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmdfayrw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3miwbtfzu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugzaxfdr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hjhgfzlt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgmcnszj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gqlfahbn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ektdaztd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tyuupnbw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ffbpvtjn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ycppbpip.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mkdjsymh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jlvcbscw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zqwqolkq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zmwzphlp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vmlxksur.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3acfdtrev.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fdxqohou.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtoszmyp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dijmgaoj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbbbyysd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dypmojsu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vxhivxgk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jjjljmdv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wqdopndh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ligwivqp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3degtvduj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdixdpxh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bxxgflya.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkeatvvl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vfevmeaj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zjtjuysp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3evnmndhc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ootmsbke.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ekucjcbz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ewyzfklt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kqvmbork.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jtrgrzde.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dobnighw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyobskya.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fiyegdbn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ianvpjvt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lafhvjxg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zgiofopl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3shmrqtcu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qilbazsd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dbgqhdwj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pashampw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hknxdnxi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xftmwkxg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wndwgdhc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3equswrsy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pnjalwno.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3htvofeoz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rizclxzx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvghmgrg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ggpspaxg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibarbgsa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3phibjniw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3apezaceu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vidcolwk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3olxwigwf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3psxivnsd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xwkmzhtw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kketvnqb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xhzdslyw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zdaoalin.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qnggickh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rnqkcgvc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3oplfyzhr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qfxmdibh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bzpqzush.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3anroicch.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rknjrrli.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pmukadcz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ryfscsce.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vzfmgkxz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jmxtjkfp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3lfgumbwd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wdunbfjg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3iqseygxh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3habtykwn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rawwhfgv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwkrmywo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uhjxpnry.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qicqbzfn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vtnyiziu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlyuxalx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bozhiccz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ikartkzh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hioyntzi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjvaiwlv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdlwnvto.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwfdzkgn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fsamplgd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ofhzvjjx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3agfvorra.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3thejnkxc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhkauol.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zaealaie.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yipkwauw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3maxlpftt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yvxejgrf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3toaqmeld.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nippwiwg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hkwzsrre.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ofjeriev.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nrbjjexq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3erwgychg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rrluexpv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3levvdkah.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ojcsyfhu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qgmmtjyy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qepgjnhg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lmrzqybm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pbydefsu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qkygbrbb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ylyoxwpe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yhvujrdj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wtponeoy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qzoyjdwp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jucheyyk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jfitcdyt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gegdffko.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ycheinqs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dobcblbb.html


<!-- 参考信息 -->