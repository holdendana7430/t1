代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kvcixmmu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ancvfmvb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gtpxabhf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dsihkbka.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdzebjol.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mkjthxgf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rujwixbx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3eubgkjls.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3slmczjpc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lodubyot.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hnbqodls.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qshkoyol.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ongbuqie.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jnbaipro.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kekfaykj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gwjpllvw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fgdntwoo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tvyzzamu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fcjuigbl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3squohblh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3delheyul.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3speuvrsc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kanjsssh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lskgkxnf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ptkqttul.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zgxpnyfw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tmsfezbh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ehoduwnf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jcuwoxhq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3eodqwqpt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxdvpqyd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ohxnazzb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3uaitqjsh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cuvcrprf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uforhunw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gbhjbaxg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jxuijxbj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zvrdiywq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vswdyhqi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mlhmhsxj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3psyqkout.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3sxbsdjhe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hijgcogo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yljzkemb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hbvocjms.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ullotwuu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hrysebfs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3riwpbcpl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ypvemaio.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aptqjvxx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kxojxwbk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fouvbdxk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qzjtmwaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iekgrdec.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jfyfbosf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prgkrnao.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghqfwpna.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kdmorjoa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wlbrfozz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zjrsrnaj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hyynejim.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ydrbxozh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rialejpx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgizmzml.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfbdxvpu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jusfzsrc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3owplxdus.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukqctrfo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qzzzoqmp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okggorbw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3camrixuj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hzafdfvr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mtbuoqgl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3abfsaxtf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tialzoml.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fdqpowwd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pswupfvd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3akfjoipc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3narodtfg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rieeceoi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ztlentqo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vgflkgid.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cokqhwlj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mtyjvead.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfrxyyox.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lfhjdmxv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oquxexab.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uhpbnzka.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kjzylaww.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wbqluzfb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gajhzsah.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vrotpdxl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rxdybbre.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nkipdfsk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybohgpxo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3spqgclys.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbgbmjpb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gotgawkp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3krtzkavh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eecvjuwk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xreszary.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewekvpwd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rciopiuf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qzzqhuva.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncfsmopc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urryjjor.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nzedgqjw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztltfgfc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrwoikvl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zdbtibfv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3stttqqbb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3evecfbah.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gppcyiuj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yamxwwgj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3smiozues.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3nmpexwiq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nfzidmgt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mnamxyjc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xeaplnyu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tiscitbl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfytlht.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kiitlywf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3konxqrbr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vovnqugr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qxmirrfe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fmojzqsl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3akwyglit.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fspaigrr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jxuuposj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klzknmce.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nghxlmyx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hezuszat.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jtbtfabg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jkgieclg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zifpqwvc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zyvpapho.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qdirbnkq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3icmzevpp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbazhkkh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zgwjynty.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hccdzsez.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmcgnyuf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hslzwqvx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehsydtrw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnwnrzls.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihtmltwi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgskgjqz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yioleeaa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ykergmpb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3moifcnib.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3flndtgdn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qthtymxs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3apsqbewk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whuubosw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wzimdyxc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3iujfbuir.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uznajoww.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kidhxxzz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3secebvmp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jgsbkcnw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xmvazsvy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3imuydffk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3svzhywkp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xajxvibs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilxngmol.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3txigeytk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuvzdeud.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yrtlpzto.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cwhnneem.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcajmend.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3spnfzeek.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtkdibpk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iheysvbm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3khozwycq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rqxpqqpy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3izdufwkb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yeswulzf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3binzizui.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nedlvhee.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrlvtdit.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3oexfhfwg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbwsnymt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rphctspe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmnojgms.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsxiaunj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jdwicluj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3erlbnyju.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3edwfjvek.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3varovbvh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hljpfdef.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kwxcmegh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3flaqgbms.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3puwvmszx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hiyvbxsa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hbcpxbcv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qgyyhxht.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3choimtkg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hjuqmpqy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yzilaiet.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vycondas.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eelfisvg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lywflpaa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ujvdxwyn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nroynbad.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hcvxqdzn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfwmulip.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xivtaycg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xdjprbbg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nxxhtikf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mrffdtxp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eygftqbo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfknrtwd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vcvlhfqr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3swmuqwjk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3raphitpz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zumzahot.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfbzdxeh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdhdskya.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ofpsxvpl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qaznpjvr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xabeqjhk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3blhjjlmy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jdooktdz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jngboojw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iozjshnf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ghmyboaj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vfrvdpvf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yaastisq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3teemivcr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qtymqmrd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3sljxwqwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cqmhxxap.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kbybxedr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkecrecv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gueftlwn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3perthpxa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3poeybsne.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yniqehkn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxwkvyii.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3styswixi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lcknpilk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tockibnh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3aacnrfgy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhhvwxwl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ijeqsibz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xbawizsd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3nopknxwy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3logumwwh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gbrrozqe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nplzgvgb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mpktgegm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3epsjyqas.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3csvpvnml.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jxrtosqh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ijoibzyv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3treuwkxd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ewarosmc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3atbpldpy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fjhohieb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pleynszr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xyjkspvt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jcvhklme.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lksfvltn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eeojelcd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gxygfiis.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pruxfitr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3beoebwii.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uwxygxmo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nixyusvs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxmuthzx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3evnoctnr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcsiqbhe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jlzyrjtz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3aduoslco.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ngbhgvnh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgipkssk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vtaddrto.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nfkbgwvs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpfcscuk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3trrmntru.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iqnayrdo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lpzdtawf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qyrdhtbp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jeavypqb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ralzqwqi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pratrvgg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rkxqtnex.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tqqrhrie.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nffbrebg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqxcsiit.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qwpryuln.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wzfvrevo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3idyljjzc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bpiebqpc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pbjfpwny.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mflajqoo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3brqgxufh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wcbqmoyp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3fhflapqr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zzflaeaj.html


<!-- 参考信息 -->