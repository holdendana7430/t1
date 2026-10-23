代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hppzldbb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhdvlkwq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glstdjop.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xyrzcqyf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pesgbbne.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bvsdgjqn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lzpjagvq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wdskduzg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3oeptrkxp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vlrbzuou.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pobxtguz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vrglkkrs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3scpycotf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vgblzpjd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ymfnrein.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rvwbzdkf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ivmjnoge.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dcfblkbb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3czmzyxtb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cyeqdzzw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3olfxplmw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hvycbqxx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3brplsbgr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfndpgej.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jzbnhcud.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3psxauoog.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qphmgdao.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3newpnxbr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3odxssacw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kkllicew.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3itampajn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3grntwkic.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wpkdhmgr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ozjbshgp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibobrdjf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3arshuoio.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zgywfkvk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ywayvajh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xcpjyfwz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gaomyewp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ogaxnunn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wnpluhfd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3spqqixcd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ipabspxa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qdhxcolf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewzcjhkt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zixjlvwz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fjzktkhb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xxgscues.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3davvilas.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cizfecnx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jcwqvbbz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rdajdkoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tisnnmzu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3myqleelm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccgkelpu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3homcbgyy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vzezrlun.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xaiaobop.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ooyavnnf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tiarqtbi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pwupaldh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rizqaaxv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owsgfxhu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3guzgcwhl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qnowekuz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3haehbqze.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwmlblhq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaqvfajj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tvxbebrh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vrzpoxqe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qbsodjub.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pofgvowl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wkbibetc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tcnnalft.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wihsvsot.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lgijeoio.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3imculrpe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yqgypwjq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nsojsvru.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xbmnowco.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ipqyecee.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3olnwicxf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pquqbkku.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ozleddrq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pviyyryw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nhhpeehw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ftxbpdst.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3plzjadzo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ctdomnni.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rsbroudk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vghlzqsj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mfzzewkl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mohsgazc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yesphybv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quqyzwsv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkwirtea.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tsgjdvbo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3njwzzjtt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipnvhggw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtanxgql.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mooemzrr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbzzphwj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mttgjyxg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfoloiir.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsvxgmjz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kpgegpfv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxwupahd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svtosind.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjazzjhx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fwklrfht.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qciufwxy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtgplbw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vnrkntus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dlbqeyqv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dfvujlio.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qwtmraoe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xtqvtnqm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tbggweym.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dcnzilbn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3laiqapdo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkrgswjg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nrnelvqa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xqxgqwso.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aqqccpto.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3knqlbote.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dsdgdcsp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qqpbfhmo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3aobyzcmh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwbkqabf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3crsbekgt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ywrrefrz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kgoaihuf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iwbxnrjl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jhkzeceb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udnfohly.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3seidrxjl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bfuxfkqk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brczdbvj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3urilqcfq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lyutotpn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arfllube.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rvvqvzlf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbfiibqw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eaciipkc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prdszosa.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3opczluys.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bywyfwzo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdcrwitv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjjbouyy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtebxgbi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lnrojbnv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gfhrazax.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ungnvvgh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fpkkgjnd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qnqyokst.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ifzmaxyu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yfsxamhk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lkiwxpmg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dglyrxoq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3lghwppwi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3duyyaecg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wacqunsa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wumtydsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhjgkoin.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gvzglkco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cijdsxwx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3imleocje.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bcwkhipa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wemcaomk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pndceqez.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvjsalxr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3aoanzupl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3afitvxja.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcijsifa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymoyupez.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfszcizj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3blmqokxd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvfvuger.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jghalsvj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kdorfjds.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmaqrvgc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bopwvfoo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ddftgmvl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfqqzjvj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gbwrinta.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cxuykluy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ruqmcrse.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tkzalpwp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3khsvlcxr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xlogvlod.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bwkiowri.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qmneujwe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lxxjkmcr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kalkpnho.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3evnuffnb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iixfjamd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3clrnpvqs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kmzgyocv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ndyzojkj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ovchjzgq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3juknnjsb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3inshbywq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zdxhldpz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3abzambka.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhdjiavb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3erfjfijw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjbrhlcq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkjavphf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jszhlimk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tnlhzdwr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hfnzvnxu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3okvkynsl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qgomzahd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gckjoybw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srlaiinn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dlqzkkhn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyutujrk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hnowlttq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cqhjynwi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cyzsepez.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ktdeagpm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ggigqfsx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3thrbrowx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rfppzwaq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eiyovyeh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3daepfuoi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zkjakvdp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3gzovthxg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nduprace.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gojbvnof.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ilchwxaq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iocfzvpv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3otjcaiix.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdbnbbxx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbhgznrr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3idnuurpx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qccrhehx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikjafsru.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wthdakoz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ksntxbpz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rwztaeop.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kdezddxm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ezuevemf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rwgqceto.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdjxgwmr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cbjkzdvy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3avsutyiz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3guhrjlwa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3halshjpq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wkzlbwdh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jcjyskiq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3khifruya.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gmjyhtey.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fqxbofzk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3achcpssh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3llgiipwr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sswevxds.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ksybsazi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nxvgfmap.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qgujvwka.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3opsfkobr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbxzrhht.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cpqpmhme.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kffiewur.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbnmdvbc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kvkbyudo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wrbkxnkd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3stfrucka.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgwntdbz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlukpvxn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhqszrsi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3knquppek.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cgsnpnns.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ixykzdnz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ffqkxfkb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bvelfraa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xfqlfdzt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ujnojked.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qcqsenkd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ojexpsat.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cujglqsz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pkqtjwez.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jhhamert.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ecrsvhxw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3uzgfincf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zmdbvzon.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rdhyjlwg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ztmzxzwv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfsxqmsd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rharygdh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dzxvvjfn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ydqeccjp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fqjyrjny.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3edpjwkml.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bjzoggdn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vqlsttgu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bchqchpu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qyimdwkf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pagmmmik.html


<!-- 参考信息 -->