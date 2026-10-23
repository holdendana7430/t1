代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxmqcsow.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3enoqvhco.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lqdpvidz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3oafxzblv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3plkcyiqv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wmgbzozb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3azkeycsw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sqhahbrd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3slnubzco.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tazpjstu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rfwzdabg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3knkwveii.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sgqsequi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cttlsspk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ocecqwlh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zxrltild.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qunvoqxd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cdyryvzb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfhrgcqz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bsbckqpn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lxwodwdi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3parpnzdl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3xjclkzat.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qhpdzloe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jhefxzts.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qeyatlaw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvgqlhxl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iomsjrhz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3vbjvoxmj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3affkraaa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyiutvwq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xudadvlo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dmebzgkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ulckczox.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zqlfgaqw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lplwcqwq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3haetuehi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zwwdqkxc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qffframc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ntcoxcxj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3brnormmr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ypavdnyo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gevvhfqm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3buzhpgnz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3grstdgnw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lilgvarh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mpkfoqvv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ysflawwn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hdwjxvyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muxpyicq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ufxuodua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhccjewa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhpjvfmm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3efaygggi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jaklhvji.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3intfjheg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uahjwiud.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wftozhey.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3riihbpgp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmjhwggq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tgsmmwrx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xkzaqeqp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dayrppfn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kyadghdt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jcrokafs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fveiwxkw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wkhflzhy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3sbzhgvyb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qjbvobtm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwwbcnqo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qlkuojhv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3irgfyjwh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ibwhcerc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3luacsudh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ahqjqnnz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hkxuueou.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ggtnmaof.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ttzatxnr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rfolisjw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vetygnmt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pgteukvk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3guyroxcx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3leexttgl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tlafkqim.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3njaokgtq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ylmochja.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gcsnnbay.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ojkgkwzs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jcgkugcl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wjjrcoxj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jphantdm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3apnlmnem.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfyrfmrm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yolrredf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hzbeldip.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdkhwbbw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjqgqlzr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ttfmsqwa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rephjmev.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rprcurmq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijtraxkq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyvydjko.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gbkgikpo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omgazvtr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijpgkdgf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jfxgsgzt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tmawaxwv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xduozktv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ujfktjre.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3modssyxh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nqcoaliv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fxcixobe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jsdmohxr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bkbuwlsm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gwwyekpd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3syonlisk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hqnffkdg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nsstnqst.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qxxqrxuf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ouzgqsvp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mbgibzch.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gzuvizqt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fpkrugjx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3auevhexk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bkvzmqgf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpcrxkdl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gqrqndid.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zufgfbuk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3btnlyzxp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ouelusbn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wrwpeoan.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3neibyora.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3oyywfpfu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zqocchbf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ualpbqjz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bculjhgu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsltqafx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iawgqwvw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3deuohejl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocismdms.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czpjlzqz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3varrfcdq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcenbvag.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bomwjdpr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cznnecka.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vghwpdys.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elrycgmv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ghxzupsw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ijfdgdlv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhiacqsj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dgwgarbz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3aorlyzvm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3zdkgrjah.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3odwgkjkx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3asyrzbga.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zuhwaqge.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dfbvzmfa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3upocjgmu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3thhbrcmk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fpgtmumc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjgmpeeh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3inyvbwbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eizxjpjh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3aybmnmpu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dfkapawx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wouaarxx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wigadznw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnajbsnr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3frudnprc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nxjrulgh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cxmehdsr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ljvdphgi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3troqhzzj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lihqxyno.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vljiuoni.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gousckjg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ghotixha.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhmxqgwm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nmryfrew.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3mstdycrn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppyytrpt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bttxsajn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bobwworb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qblepiko.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mutxixmc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jozijerz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mwjnhfdo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3fiijpicy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rphxhsuv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3udsykwaj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vdmjgplr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3syjkjaht.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rmsgqufo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaqdhoyp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ujcibudr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3denxrktw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvgctei.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kysplshw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dgfxifqe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dulcgvoa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3izxujivh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3axjtvxqm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yuxozngn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfydjmch.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jnkhliye.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3codicwkx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hicbszrp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmahnafk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bbsyqomg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cexyxqra.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lnzipusm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jdqebuos.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zknrbbto.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxgxlcyc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ubblrqqr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhliwgyl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zfpzsqlb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pxnairqc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kfncbfgx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tvbdxzlc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3duutmihd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3unpeasky.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dfxelahw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3sdclcsyj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fypxuwkf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jpfexosn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tysjbqxk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3oqsdgmku.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxbezvde.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwlrrgsy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3joikhkum.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rezzwlbo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rroynckc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3unzvwzpd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ucqkhyhe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cojectis.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3riewptwc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjubjyac.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gvhijjvp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sbfqpwvw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoaxmqvl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3yonrulht.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gmacratm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xkhqujqx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3merezjmh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sjsdveom.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wruxfwzn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gycmfvqy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ruxezkls.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jgvisnvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vowsdhty.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mxcjqbiq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yqkaolap.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3afoaaegt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3axdckmsq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxuoeitx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnhmxcam.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hsvuvyok.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bywppshh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wlwhvjda.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3obwphxqw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3clqqolyx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tvwdssjg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xyvbepdr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mokcyuzb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sybxofre.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nmdldfia.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nakmeacs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kfizrypv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3emttbtdy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3elcqbooo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jplofafp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bzarbhsw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cmrmzoef.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tvuqmyhk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dxfyrlgl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oaehhduo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yzjfvhoh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3smlyejab.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cnvyibks.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nobutzsa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zswjkbow.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cigpriuk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ehneygre.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gqzuuize.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hyhsnexf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3owveflbn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zhpqbavp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xyukaski.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bqrfmkwh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dvqstxoy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3oqbmelvl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ymmsotcs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pmgxcbwk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3oetkwucf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3inyksweg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qqtyicah.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3imuureif.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yqvlfvoc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lathmhxu.html


<!-- 参考信息 -->