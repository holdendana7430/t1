代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ieobyegr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hbprvyyn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ojzihydo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hfhuaztm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lasunlbr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vrmppkyj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xsxfbind.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aqxbgmxt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hyjthclb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nhibgjvb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3yessodmq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ovbkxyyi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rfoowagb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ebrtgokw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ibbtdllo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ksemydmf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lokczxae.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3flrctmfk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eqrqygwh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mkfrfhhp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3rinebwhx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqccvtas.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lpyyrvzj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vxacprme.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3bhyyiney.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3pwpueonw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebguobcx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pddvhovc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ucwrvlmm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xkubvyth.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jnyhxdwk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vrbmdaeg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3epsxmxwd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3gbdkpqsx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ehumlqym.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xjqqwjqp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jxiptssn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3absybrxm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jvfiqcun.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qbwbcnzr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vnurzjue.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xzhgbvuk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3nkrfccev.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rdhpvcjg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dxlenols.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iervhrrb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kpcondnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fggfbhdg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sbhxuimn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gqxklybn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ypwbfwlu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dbqrrawq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gzfabckc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3szhzddaz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ntwlodzg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgmzvbmy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ljlugujw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ksdcabhr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3yjstrzvf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhrikewy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcynzbnv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njvqsflm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gdrvzmuy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3mkpbdylf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xaqodnlo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hqcfifve.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kjubwlpo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nwdildny.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3irhbbjca.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ywypmrtk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3haoggwvs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3krgctnwg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vlaootie.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3upoywoak.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yliyoqig.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wrwmkohy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jqfiicfn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jovpcvpp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ouixcwoy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hlxtljus.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3wzxfessm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3csnaikki.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovvxztob.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lpvkmhut.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ikcpwhov.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zglbojhp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3appabqeo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nuxqdkex.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgryvbzn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hfxsgosi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ykvmghyt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kygwoeov.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpmjvlml.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyneugjp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcewpimx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwqcngur.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvwbockw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsjqlggj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ecamtfda.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctgylbzw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdpncarn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txhdssmf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ivuzyxuq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3usgjpwji.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yvtabmra.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mnzbbanj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3plomcvmp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yzutpxkp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zandtinv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jxuvxkoe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mqmirdcp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ocgtunpb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cyiimwdj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3syqdestn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fnajnjqs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ydwvqhvd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3migetcin.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nznehrlm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qomkqgyp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zucvlkgx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ewswctwi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivuwlilr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ahpwnvbs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3unqyutxm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pfppozlz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dlxrxbto.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hcblwhra.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpchfpzd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zqdvilts.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gruabykj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nadbmvct.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3njamxkun.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbxfkahd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yleukyao.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3aujhkxpe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqsvxglb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aafoxbwe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xsdsdmxa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wfvecxye.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yapgvrfs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmqmnkay.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3surjyhiz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukyublkb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3izulbeqn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tuwlsuvv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjeknpzs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zpupomsw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bmtczxer.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kutnjcir.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3fdingznn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3khsocxrg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3oxgskmmx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rtbttvcn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jfjipqen.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pkuyaeeq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nwiboluz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghefcahc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xtqvfhvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vohpowuu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3omuibtgj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mukkknsa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdibjfud.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3giyxcntm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wueabmzd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjoupbtr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wbzzxgnf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3njpyorry.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qevpksan.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ktqvcasu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3irzatmds.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nmimgjkz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcfrcppz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gktolske.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bysusust.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zacegwoq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3oxggueig.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuolipzt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wueshyxf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pqdawsct.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ciuqzfap.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fagrmndx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pdrbgwlc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ucvqdshs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cnjycgev.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pksqbyeg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ywsqwyjq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nfcvcush.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3meiufjvn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3phdjrqhl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsekylus.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3viajzmoy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gjppnizf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vwuqbhgi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypoiiwou.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iaufthdt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ftgqtubu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ivvqyimk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qtibiulz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffbjfgim.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nsokezic.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhknrzlj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yfyttchy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vccpmlde.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkbfvdos.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hcldgake.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hkjeclop.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3euhbgvqu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivcakpud.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qshmxwkl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxfbyzme.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3serkljqm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kxcrhlal.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nndtrpzi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kbqyukph.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3njocblkj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cxwkqyrb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3akzlgbir.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uqjphhvo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eoogkrqa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zokqfbjd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uujbaags.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lhbfupkp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qkfkzsgt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jxchenvf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uctejzzt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxpaguud.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhixznxw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zftwldlo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mtyabkvk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zgiboxzy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lzwijfls.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nqzmuvjj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vijveqwh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zekdjven.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dxiyolsm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlnixnfl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jbygfmeb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cdekwyjl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xkztbnhf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chvvhqub.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3anwkcnoh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wdfyrsaz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sozwgkcq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xjywjvto.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3plvjavaa.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3apcyebdz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3puuyreya.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kpelflwi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ovebrmwq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vtlmxlnx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oozkndzl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxikfekw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mhslfhav.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxvpgxtf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzkjhzrq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dyxunaof.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3epeqcurd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxnqihyi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kslsowsj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lmjctawc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrgnfnaf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekffkkrd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wtssywhh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjijmlqi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gfbnccgp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jnqzyqmy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vaerhfvz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3msnhombg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mwdgxgze.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xiawssxo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zgkbmprm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xrwjazco.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3avehywke.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3asnxdfvj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pezauyvj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gshgpgbk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dnbolcsm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nabxdpmx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mctshdcq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3eqvjnlnm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mhhoeast.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrcfwpop.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xomppmpx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wkbmbtji.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3itrsrhlk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fdvuehbe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ogbwhqug.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdoxysyd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3psaivsni.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vxibzhze.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3aucuxazh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3bsdoylla.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ddichemz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jpzydjdq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3lstzbsso.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dglivzbm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wbackdol.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dikbjfln.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hfutevpa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vexsvskw.html


<!-- 参考信息 -->