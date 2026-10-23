代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pabkfsup.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wltecsos.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3drtfayyr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3amhgyqax.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zfpjzoxh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tfouitjm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pujwmjkz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yrvrwqan.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3macohvbl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ctoyczgv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ldlrmwtd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bwtzrzoo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fbvotizv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lwfffkun.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cglwwptm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zyznpwty.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vhiqgcmy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sabfbppv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yojpdcjq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rdcalnan.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lahzsfil.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jbmyklnt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wshjtzkh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fqjtcadw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zayxmpsb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cukwgcsf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tmjodhkg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3atzwdcfc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3idsuqotw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3udvvmnzz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wrefhasa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jkvyxvwj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dkrioztc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwdepws.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wlgjmvwi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bhnbxvli.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jupozqfe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3hlhcdufj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bethplds.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ujyrikkj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3janmftoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhumlucj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mbcnabfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puzmcznm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wchkhbaa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gyxndecu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrmcncvg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tjakxwzy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yjiuwocj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bimkkxmd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wpfqubsw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vytzsaug.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oeqteohf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmaszvhe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3anukhnex.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3evsksfql.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hotfvodt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnomwrlh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ujduxfdg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kivqcfka.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gaaqstau.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3btkunemv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jrftjppn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3yinjqndl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xwhdfgvj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kxcbmmjy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uukbpcsq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vanykrgb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3esyyvoha.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fpbihdxr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3slybswqv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrofcasw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oqcfxtmh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eocmeusd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ycoieoia.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mfzvzbgt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bulaclos.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3duixtumu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uceolnhq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bmvjwnyb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nlratuka.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zlfmvfko.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nquynuil.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqyuvrsn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upkriazy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dslrbwht.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lfbfsrmc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elxvovvv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkdnpefz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxadtzrb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnomonue.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rpfokiym.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghoiwbgg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqckiotr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ytsjurhk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kprjgbzh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibsblkec.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zhepwrjf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hbyvkzwo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjtraku.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dznrqjex.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bqnrrorc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dkfipicx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3icbpqxbm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mzfudqdd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kvxczgxj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3axxiqulx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gdtyqeeg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3famcudgi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lfbgwtsd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rdjqbixg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fzfkrhds.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3elzocysu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rywldovm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hcpyzrep.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3swxaeoyw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ysepwvol.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fttnnjzd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3czljiuib.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3aimvheng.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kwpmmkae.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cpiydclg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3owwegfyt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvwbnyll.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mjkjsuqa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rcorxhlg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itottkbp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mgnqxlsz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfjnopxp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvyuteqq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mhspeboa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zuzbxwvb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tqxdudfs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwfdwool.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nqfgetij.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3quvvixij.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xbcpvpbu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3umzlwjog.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3btjgzvvd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ahthfswc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zrdsmgzc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sorfblie.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3aejoopaa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3frfviilo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xocpugcf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cgoocixs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xmwggzse.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3memexkwx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bnznqfqy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pcpyupop.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3picxjghm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3shsrzxiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjwvfvgd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ivtftdcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvfcwnic.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fhoxevdk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zmhvcwbj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lndcbzqp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwtxkxoq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3axdzpzlx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zrutfxkn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ipqezqmb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xgzqdgmz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ihtcsihs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hilfgxnl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gybvmzzu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlzroxlz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kgnbvlri.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjwcqyqn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3asrjdjoa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tfcgtjvu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kwfmqnxs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrhexcwp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ksougnfr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ofkextwy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tqrwjcqf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pumotwfn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tyakxsgj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gwinmkyy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ahmxsvem.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jydgbith.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3aueouzil.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gllavlji.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zwkdzcng.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ohhxcivp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oilhrtle.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tieannjo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xvzriykm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3milvtnhf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ycrfzihv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rjomctxu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lrihcate.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wulvmqcc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfkczyqw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xobbuiss.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfvbppea.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gurieqxe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3appmegtw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbapklwk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgsirffu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wwtrabth.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3eeqbuwbu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlizokwh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtlqsbqt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3atijgenv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dfecsxjb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uhboljkk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqqboytw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3padswcfe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zyqrwoph.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3odxbrruy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xrjueujb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3moudtnmw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fshdsiid.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mhxcujhd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3znycpjoe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bejiqsvn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mlvqvply.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ruyobocd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3oyataiol.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gkpnuyjb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxnvsijp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqjzpjvq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehjfdkns.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rvcgddch.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hptspjfu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3homrfaxo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3txvuhcsv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bmtvblbn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvxemtid.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tkeiipnb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3faahhbiz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mxvmfsum.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rramffpl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ayizzhrl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ileqfckj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uzzzshjf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bjnzjuwp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gqdjcwqm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dwplafis.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jjqadksc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dmzxayen.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nsganszg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bheacpeq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3guyeriaj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3snyfoudd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3eszhefmk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvogxmxd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlcpfiaj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lntfxkyg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyfpqzsn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wultupby.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jssqnsdk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhqszecc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vxvfkncm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fbuwciff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yivjynvv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtahjeas.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vlhkzlbp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iszzllme.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fvukudfw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtwqqwle.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hjmhhxcz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3yktofdgz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3whxdpycv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3khjaadnb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ecmscjrs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yczbcwcd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dutmdjhi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bthvuben.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3cfmaonog.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tnzfvxgc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3crpndhsb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rmfsbhqp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3iwtaowlc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nlwaksmh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3izhwkxsn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hneeixjc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nlwxwyow.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jbyalnwd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iadbqqtg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dhqnywyb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pbazvdvc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fnaobcsw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zsuowdnh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3itczubqh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gjwgtzwo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ttkbadot.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ymmdxjle.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzyayusc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3uofyfxwz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jijfpnsm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zhopigng.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jwknwddi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ohhxwigh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qmprrxwd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gvztohka.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3yneovppb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dumszmll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vigwpoaz.html


<!-- 参考信息 -->