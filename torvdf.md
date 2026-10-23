代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztanofuw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pqznjiwr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yrfnictn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3nhackdee.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3twvhgojv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3jzpgfxkp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3saxazrjk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3diaxwbby.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mwhndrzu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tkojqykz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eciqatws.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vzqkifxo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3knosbptw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3sgghxoue.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rmkrcwfo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3roeebase.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3apkkhqbd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gndspimc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3baukblgw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zpjswmdf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mbuhmvsj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wyxzxfqq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nuldunud.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3sjhlhxum.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tjduexvg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3spapkexj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsxvkutv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3osfijjlv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcaijgrd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kuzafqpg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kwavnhcd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3snpjhsem.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bixuqjxj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ucgybayj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aaryoaam.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rhsgsedr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3msvjzzmf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3frhkodyx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dhygcsmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3njpzfxaf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3hvwzgtoc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qioedwnc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wdicgein.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wqgrugzq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qodzkaow.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zbbhkuep.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cddwywis.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nkcssoen.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jjecsnnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvbthshp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3izldopcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfejyjie.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qgympkwv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vpcjwjic.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nttujpyg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hzdzknvb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3btlffzyo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aexrwaaf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dlimrmba.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nuzogrgw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zjypabrw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhwtbduy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bqavcpmv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cropnpwv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibegdxab.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pnictpzr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3misfnmsv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3oegsxilx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lyxjevlv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pgyktmbt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uwjpoacz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yzbluqgd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vnxpjequ.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3alheqkkz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gtnzxuxq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qkszhfxf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vxvoyovf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cxdfswwa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dumrseuu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3itqttjzw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pspgihgx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xvmqduel.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mkaivswi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ltbzqafd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tlcrmgii.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pyikldse.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3crahqvss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3obzhetfg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ipogyudf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cajrhdcr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrxvjdjl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlhlwqjw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjysgwec.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ezyckojz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gxstravp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhqbnsrv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlajknfm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3imtyirnw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aytrvlsk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hhkoyyji.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfaihmfm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cotraufc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gxoawoxs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifyccwnt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajsbzgwr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mialwfyz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iaxknwhg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3alnkmrwg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vfjgswwh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3asbobpwt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3prtjqdmc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cxawfmqq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lvdjhomz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wfnpoiut.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jfeoodyx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fkczlrom.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3liqircbv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vekvgmuo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cweckmdm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jynpxwoa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3betdoqca.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3llccaupl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gylafxpi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tuzdjfps.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fffvavpw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cpuiqihc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3snqpdhhx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pgzmrefi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rwzfwscx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wcdncdnm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wsuqcegs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aienhvad.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3besqoevg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vdxhsykz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prpjzshi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cglbvacf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkphbiel.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlzqdkji.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vlnkxbxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbqumxql.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfjlzkdh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ueujyulv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zojbvegt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ithnvuwe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bkxuwsdi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwcfhvel.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztdpmpqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rnsqdyxx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zrqhpudk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zkzqnvss.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bswhsstq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wnsyxwsi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mlpuqimc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aldoerfx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qviablgd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3japxoorl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xitiemep.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xktfsawj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nivkbriy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zcpmojvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtkafwia.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fyutlkrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrkhofap.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3goicigfv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bpyclpim.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kdccgyxr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3quzuesmy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqnznunr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3weeadara.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3chcokltn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fkqqtrww.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jfljodns.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fyuscbsy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3facahbrg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yaihtmhd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etqadwni.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxpspogf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbtzqvzk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3itwzykjp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbjuiezx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vnfldxbp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ewzazeyk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xezinfxk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cvqjwfrg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sgcrfhow.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3njjpxeku.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hdvwbltx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ywveekjj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sohotsnu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ycgqknxp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qpbhqxea.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iwvlnygs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onsqucey.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rczktdtr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ukduncnw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xkbiiuyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zrtjwaup.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rdrvvpyt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dwcpmjde.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jruywczv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hijnendc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjcmynir.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3juawybcf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3scggafmu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkuxrsum.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hkxplopo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffytatyr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jqqgcimk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jqscdvre.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xdisdrla.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ebhbyozx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igsocmlq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnqxaoya.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwqfgnme.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ufkbgols.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3sdtxsfgt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ugoxupxi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jparwibs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3esqdrkyg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bxzhwqga.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mdogsxtx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tqwmgsdp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3clfkthxu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ukczphmx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ykggncbf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3azgdpqwv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qxvdnjgk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fdeochxu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uuxvwkmn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqibytjo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpqcxhgz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kbaoaznx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wfynzxje.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zabsfrjt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3haloiilx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wmvitoef.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fdrlwhro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xljldtdl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3imclxlwg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nigbzyag.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xfmmmjxj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zsecvoko.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vwoxpssu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xzbyhdrh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3srysmefh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ilqxgfjj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uknzzcol.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mblzlnka.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jdlhoiof.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3phgxbnxn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nwgbbkwt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3apzqtbmq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ijlawpjq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3utoilhpt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3khzeoprp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kumhyifq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cbhaygem.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejatsefz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eymtzlzd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aypeqdta.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vvvdgycj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3svjxdilz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rofqkqux.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lodfbveo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yfqpgsqk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnuasjun.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cpzvdmej.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utrdbpoq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3llmvfqtz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3albnvrgj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dmfdhzvy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3warqnrdl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ugjimuvs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3msfexyfa.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wgpitian.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vbfiddqv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mhevswes.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3pqyrprws.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ieaqxuga.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tvmntspf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3iwzyxhdr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vdvymnxj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xwidgjrr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3exqbbqxr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gruxlkvb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pucjouee.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jtpvxaex.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uaxhdcbn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ayfwiufx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hweovqtg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqcjdxfd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhtzvkvx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fxmdrvye.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ngoglikr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3taeslqsq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xyukerkf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rqeybwjg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3chyfhytn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3puqwuvkm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dvwydjto.html


<!-- 参考信息 -->