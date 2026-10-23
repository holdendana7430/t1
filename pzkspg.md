代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yqvfapda.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3atgwjxye.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hqjdrffy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ejqhjehm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vcmvrzpm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3omnaitom.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xmnuutrx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3czquzjcs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ipsfzixj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lshjzobw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cbqgeols.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rtsfpuyg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rcrlxebl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gqxjxbfx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vhemlvkx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tjyhwhiv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgakqfx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ndbdhcjf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3lxmjatxl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3uqmgkakf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3smvuvpqh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vsngcqmx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ktcmxfnr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wsylctis.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zrekhlej.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ljemxkoh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lugcvcmt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzodqmzp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rhlyzcgh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3slksqglx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qgfeulqk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3aqxcgxty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wmanhplu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dduutydq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ojkuqnzt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qmufdlhy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tgylxicu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dlbhrnow.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tobhfpqr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yfjgvoas.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nnznfjnd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qodibusk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lrmqpbqx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ijjiaicj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yqbzturz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rvlnaywb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qnrsadyp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fytxnebb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vjvtnona.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szkdhlfj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pzmhsdnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skbxrlmn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kyfdrxgi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3baohztsf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfxjawds.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rroaguco.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ehnqmate.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aqzevlcx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3emrjpicj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwweocos.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mchhtitq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3iiwmavqh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qfwohbjc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gwmprhmv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3maadestb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgohwdnv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vjnhtfdk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3iunaemxp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3oepfzgnt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3znwlmdqb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hpqmdlau.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3etqgfizr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nqtpekvc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vrgmyrys.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rqkbcveg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dpqbfvzh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3maazrwmh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fgsfwyjc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xfxkpaba.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qozbzcvp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xjzgnxef.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3yxkkdtac.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rcturryl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rvymyyyd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cznplleg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xlwnuerh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rqeszpgm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wzrqtlzm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3unnuwhcg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tbhujttf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jcujzocz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qstldpqc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwtankkl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xcxrsurc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qaglftcy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffimhtbq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vylnnzaz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3bwttvasq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3inqjqdib.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tjvlsgvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bksmmuot.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfpdnhns.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3afmvbamm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zscvovlv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chvofbxu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dxstwhxs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xqhnajjl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xwrxsrch.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dpsasusr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3morcsajr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3enqjtquz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdajqilo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qxcrijyw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kgulnmfv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3epxflmag.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kmbsheve.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3evxgcrto.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjtrqyqy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wdmlihez.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3blajrnvj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ybgazxcx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3uuhbfovj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhxtmwy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tgkeqsnx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ailstabg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vimegubg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kviwiksp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cpolltpv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxbqqa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3porpsdqq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3opxrmtwq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrzxpwjp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3bvqrnpro.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fgkoxqgb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yakhiyfj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xjhwruxv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ruwjhknl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycgxixsy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3occpytgm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlamibfe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjddprza.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vajulzrp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpnxqwfk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrpwppvj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3byioajcs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpalkqqr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pczybbhy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ilcciyhb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nsuxqnop.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjywdhfo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dsbekpkr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3gjretpan.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rxjbxifw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gmrzwdaj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wmgsxvmg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ezkwdpsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3txulxanw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oeqjslci.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3doecuaiy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cilueuqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyvkcsjk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lvqjkgfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tklpoofa.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fbjsbjbi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3eimdbixm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xgrzlyxd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bxmdbxre.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fwceolrs.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjdlnxjy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3anagmjzi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hdxllvdy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lpmrhehx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3oelttpkm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mqiebwkh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hqqcgzca.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xwwcdrfs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ozadhgqi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imluevvl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3oaasmbee.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctuhzjdv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3osjmlpyt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hwaugqoq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gjvpgwwe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pneuvtkh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3secycgsn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bpmymtkd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3exqurncp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3owpbqyth.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vtyhxhgz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xeuakhpt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rqbikfet.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sduqgjds.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqydtjjl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqukghmx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obtvenms.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mzivhvgu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gzkyaohs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zwkmvtcw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ehaqhrcg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lzxnyytg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3awnvpmet.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dckghmqy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmrmpsbd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ixwdztuh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwfkxtky.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fxhomnjw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jyohlshi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhnbezoo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xsauwmtv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jnabvrmw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3flbymwtb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qfeiddep.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3occhwauc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kwvarghl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3utaamvef.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3aedfnkdv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ckqjivka.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3husbykwo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nouvbdby.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dkukkasn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cpwpikya.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cxixcjxm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ceoywltg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jnufkwxm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3sbgzrhqr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rgconlyg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zoliashx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kxfgoiba.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3imrnmhia.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fqqlslss.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrwscryl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gistmslm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3sktauyuq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zcmpuvuf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfbrvhrj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cudhcrhj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3blwikwam.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dmsfrrcu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3blahoytk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qpvkzlwl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmmgpahg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3odfyyagx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xnywjcsc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtadsnik.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pervzuas.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ntzbteeb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3acupowip.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3djuihctr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qkydlsoa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kbwrdpde.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jwpiwyfk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rsxrztqv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rkllutwg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yichywgw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3otfjtsxa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jcccwzvw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kmuswuai.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hxffekeh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvcqmgrm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3khgrisak.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ptjkfzhu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqowkrem.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tbbocgyl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fpkniaqp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grzzkwhy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ueqrqghk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3coowdlev.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpqigidr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lcayjrwz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ohcxkbgu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xepkztdq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ufhgaxfs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3bblxehhx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fdaqolsc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3utfojiuz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hcnkqwqc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ffgywqdt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cunqymhn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qxrutyck.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3crxbvglc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dlkrsxls.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tyqgcreh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bvrygxrt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3imwgdbts.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gsujekda.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3eveqpwii.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uxfueces.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xsuihfyb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zpvmfvew.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yzksimji.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wcfarogo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3miuyygkj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bkyisoxa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mdpphfkc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ttltnyfl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rhsscooj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bbrcuaqr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dytscqqd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3oaondfmv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lxtzqypa.html


<!-- 参考信息 -->