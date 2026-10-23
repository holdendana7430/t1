代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3trlnajaf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cenqbugm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3xvbmwsfp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fnggisui.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3maitmfaq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kmvrvpwe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mhyivhfo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3udskimjv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gdcdxgwq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nfucxomn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3aqvbhlih.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vdwonpng.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jgczvibq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3whqwtiqc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kgvuqaxw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mhrwfhic.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ythvrbxa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qoboqndv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3utozjkjz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3injvlxsm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqkzxscn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cyqofudy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qfchikye.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zyalpazl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbqkdex.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gxoupjju.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3laxtbetm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3smcfidcl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hazfipvr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ozwftpqe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3hewewpcr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3awjyoevv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tycicser.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3yrmrtesd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ledszsvt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdzytyrh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3fnokdnzb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hjpmdspg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szolttmf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ttrwvtnf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uoktjycx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dmpnocsy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ruksvcdm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3usjkulxo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3efsqpcgt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3sfmnbysc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hrelyzcu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3skzglcxf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tdvbzlcs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3inisahhy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ozbpirao.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eumnanqg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lxtaulwq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fromtdrq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bxbspivf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pspsaqpm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kctblrun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sadjypwn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3csdxiezp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiubkovl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uyxpcxwy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vtievoby.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bptvzabw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rdkwmvad.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uoctqwhp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bvjaigfx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bzpvhiiu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3itjcstae.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fihuvhfn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpuicmik.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3draiwhhe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3admzovfm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3morcdmfr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akzihbdy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wpaicube.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxwtbwic.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bkoaoeol.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfferije.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3crnxfwsv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jmqwfpos.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lgeabfuu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rbstnadm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mjnentfx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kwyjeovf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nrpoxsvv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dkmnkukm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cvhzwkwa.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3enhfmlhs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xzoaczhn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ybnkxvlg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vzlrqqqw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tpmqewxn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3sikemmou.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yxdlpors.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bzwudefl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zqnxrdxw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3muokqewj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kgykbckx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3spejmylf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twkcwqeo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvnkjkbx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xjofjaxu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qyriddih.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvzxllfe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqhlctmv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3uiraqbuj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idqwxyux.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onqafdzk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmqhyqhq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vyblqjfp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bvwnmdkn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phhpmkev.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quomitdi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zfmnnpob.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yojlwxcz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ldbfzwer.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3euufoteq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xvgnmskp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3awkwuvzu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wbxdngqc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jrjvmjjh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3blxtxosz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wqweccxs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3sdauldkd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rfccxrmu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uukmgplu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xmpswbjv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gmchazbu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tmroxcqv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3tdkfuvbf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eyqnwvyv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pgcekcgv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jpoyjxmw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqyujihm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hkxxrtjh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pbxlxzyq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gnauapzf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zvushhkz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ijygmfvm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkhpkxqc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3sezllwca.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gioaaohq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esltcdjz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ieunopqk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phnjotnw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdwtjopi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qxknswfb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdxavkkg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wuqdbtot.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hotdmflj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wtxfmaom.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfooxhhn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tfhmesbk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuafaxnq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrzrqjas.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jilxhnxi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rwehiwpg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3siwujzfe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3aajmbjse.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bzfklqrr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hfkursqw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fcoauvdi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3otqsqqhu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lgivwsfm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ykdlhohx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3gorvcklz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3impshmhg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pzmzowtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfdafhjm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3atydfggh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqtfqxvg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hzjknimi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hznslits.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zhziryyo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kemftlst.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bdsiylcl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3afedgxko.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3odkxpryl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayzfzzqh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ajlpexwo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yoborsnz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uaevyltz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3grkkenao.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mmwffrds.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3eeopwbss.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vbzfnxnb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxmqqnu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gwjikjcg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjzzsfix.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3iroukswy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ptwxdcts.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kbdvqnov.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3paoojmez.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dgkifrxb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xakvdsqs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3whtjaizt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cfptxlqq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vtixmrkr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pahepiwz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3caurthnv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzsfacmd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eeftlbdw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xivkjbbm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaymrrha.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vffovwvf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xumrgazv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cfsyhrvv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kpzerlss.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tgqwbyab.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zqrkxgzt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpdbgmte.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ywevdzss.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3diwdchpj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3chqhgiub.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3faidqgod.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jxsgewiq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3oywjijie.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3phhvtiwy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uadbcjde.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lhhcqeub.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3whweewow.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfsnqkhq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rlnelgqi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hdqsukzr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mhpljzlf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lssfakww.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yotpkxtx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jcpkhanm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3irmrjdgh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rttrdwzn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bekqjwwi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wkulmbcb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3awvtpbzu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bqodsbsl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pnocdatq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cbhdpkfd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3idiaddxw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3potvvzpa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfkctkut.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcksgltz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3eispccat.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xjljavtn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3onsqtezp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3azesiopi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dqajlyks.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttjvxcyc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wkhsexrz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3uihyqsax.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3okwpjtwr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xdloenrp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vtjighpl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ietcummb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hafhhwsf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hebtoflh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3adwxqpqe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sixqrebx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mqzzbeyb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kyqnikqr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jgppeapq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ceicmdhs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rrkusuyh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ammjdnxu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3azqcjsls.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otvisqud.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvbtjumh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyzoaqnf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbclclrk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3soigidza.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wscvqoqu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xjjssvtn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwwyhqae.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vmfrvrwg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwvtpaaq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uqbxzity.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bvtalwoj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3miwzjpmd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fjbxmtkc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3utredrlc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kqaownyt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kcykoboj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fbfxyhev.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3skyshyhs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dhmjrtmo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rfngfxiv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ugnycvue.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mdyajhoa.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gfwflqym.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mrkbifsk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bkaxupux.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3drnpwkpn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3eoyzbetx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kipqegyb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rkthukxh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3goaotpbb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uaojzvaf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qlpyfmwt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xrtybggr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wqsqkcyy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hzfzbzck.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gihdzubb.html


<!-- 参考信息 -->