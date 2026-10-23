代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlkfvsrl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3icdapguj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3epyjuqyu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3sqombfaf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3awvgbksu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vvzgxtrs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oszdxuct.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qsqzjidp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mwddusvt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oekhebeq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oeuirknm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ckinvqaq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pmerrzmy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hondigfn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3twvsjbcq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xggrbbul.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3spnyrrjg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3drhlixye.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3spxpaanp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dhdjgfvv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rpzbrgza.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lxyhnydq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xpbmdebq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pfzbyeys.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hjtftjbr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdqkfluq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbijqpax.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orymbodk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hqeglpwk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kpfaywmz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouqeplyx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qdynhweb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fulrcglv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3htlzhhqu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kdozmpmq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3prmbchmb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jwcyzmsf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fkjvrouh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ucylhvsz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wffsmmuf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3kpnklkmd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dviquzvp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xwkdeboc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dauatwek.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wfarlcdi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3llkssvcb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yavxigkl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tfjeeiwp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fxuorqxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdvxpkxk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fjofqnse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mncsnqwq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3paxwxjro.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rowfbzrm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ylyyjoda.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ceqpklpt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lweqhafg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wckacxta.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3eqkkacos.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgxeofsv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yekiwpqf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qnnlhyrz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ldrtbrmp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sgdzmivg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpkmudzk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3orcstnju.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gojlsrti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dltsvshl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wattkzqw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvtrvwbd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jyoecjsv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3eloavnyk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ljlhotor.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ukjayxzq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uucxiufr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zfmcansg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3oaefudsq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vqofrxbv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sbfnnmsi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gwvqkqmc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xxgavoda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lugyqini.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3limxpajw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qidrilbk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hvasyyfn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3raxgksys.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tvzutouc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tlrwomdt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wfgpfqgv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xxeatpvx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wjjdvswv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxarcmzx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3seujfmpw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pjkwuzex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pcuedyjd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdvhfkre.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3odpoqouq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlxhwfil.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvuyhsau.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkdmtnlu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzmhgmxq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zskkplkl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3egdvncir.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbgxvdki.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtgkdrgh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rjoesfjr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jivlwkzk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gjkzjwyl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ewhzbnqo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eljeyaae.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dobsvmbp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtdtzppi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qbapjexz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mebdfegn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lglakpok.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yihctysh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fqzomgbv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kjhnsnle.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghjxteco.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bnzzyksy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ofdjdgyh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bgszkxfw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ameowgsv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bfhjqhnb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zhdicocw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imhrxvhr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ezsrefhj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rlotpatt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3inghuomc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bdezksvv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qhcpjkxp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjwyobrn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cbfsrixy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yykjdpvk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fihmiotk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aeavurru.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhaehaxo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tngiyfzh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tmpxwkqw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnmqfent.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajwcbdml.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3torgrdqf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3aukhadog.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3roqhxxrc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3baywmxma.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eafhgsdg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjvdoehr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wncfegwx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mhxbsnpw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtulkdkr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3sswoohfj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rwiolypt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3virhjmaq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3adlrpjem.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qwflcwnz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hforagzr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3iwnwfndu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hexhqucg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hgqfsrdk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pkafcqcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pdxpwsys.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3acpnrdgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyvfpihc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cjyjazdl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3uviumpsr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dwcnyzwp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iofiyoch.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tmkiokzr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uboagqrn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zjcdxvmo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvgchwgx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rntnzdpn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wenszoxn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wfzvqqxo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3myrnbtnh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htskfkyl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkneqptf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hnzoopyf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jsucbqfa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3njdnjqhk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpfrmled.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rbtgmfei.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wihdyfmf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3blrhmvwk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3luchjsjy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3virgoguh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mguddcia.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bsewoezp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fxndutdf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hnzfnrpf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vdafasaa.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zsmpvphy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3arrcvnmh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3daavijqn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3biudxzrg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hrovuwzv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3aszwrbef.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jfswfayo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cfisidug.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kkueihff.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kklxkfko.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lsyrzwnd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rpjmbmhs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qorerdhv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ixtaqeeq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ntpljykf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iyyfkozp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yftjmqmm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hyydepbh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fpticlyb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uaxieyth.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vkpmtfmt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiqupecr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrkqwhat.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uoxhoylz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xsvxgujj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3obojxcve.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xwepobao.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3awccyjjm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jugpysfi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3joaivzbd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ogfajuem.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vvpthgog.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pmmjyzpo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3shskusrb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dxakpeaw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fbgknwxf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dxnftfae.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ueeelkea.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3titekvhm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mjxzmuzs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3whjnhnpj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tgutuxee.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dkzqnrgc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dwetxcsi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xlhtvoqi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dzgiwtho.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vjwnocsi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gdrwflpb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3szjadgsk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtnuovcq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jwqmieob.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgbpyinh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipgpsxka.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rwbwacpm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ymjwxbqy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ulpgasjq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hpuhnppx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dsmwxmft.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cttcrzev.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hfxmqzqa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3omqgrbyq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pjzjtgin.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3oqdawgwf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ddbphyau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhxswbvb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ngrmpcwa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hbpucnnq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3arilacmg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rsgrktcv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fnsiaqsy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wjcedxed.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggfuwumd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3elxlujug.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gwzluoty.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nioldfjw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwahvmrn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fvgzovri.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qmnayyfp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yofdfktw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sljebbje.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3aggmuxgo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pfshyscl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lrwxtatt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sucypcts.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dffwwyxy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ngxnjxai.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ykjlgcqi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kafyzonl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jgtqxklk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ofnsalhw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3fkiwrvai.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zslvckky.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jgbydosz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wlnyafyf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3djhbgfyf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ntvlcbhu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uujubqdn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3adeuzpgi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ppkxnqys.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3psmgbajm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3grrvrjpi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3uvbynpcr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ejoxapsa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3xutfqwsx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3crfsqaiz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ocqiyhms.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ncfrrbda.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kylmdjii.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3sqrthgmr.html


<!-- 参考信息 -->