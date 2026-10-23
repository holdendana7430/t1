代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mhrtfdqy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qornzrnf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nnooqtps.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yjggxyih.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kufmoxhb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3engcvaqp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nwgachsl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fddacmdr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dsvxxydh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rmsepdim.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vssabekt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eengznoa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aphbfaoi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ilivbedd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zwtcuecz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fjspmdct.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yglbupec.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3emuvjpws.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3epwihfnr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hyqhgxmk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mfvibxic.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3krmhnpry.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qmsexuii.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rdlvstjz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gymqsaya.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3cjtmlpgs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3alktogcx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3utivziop.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3phpzdxlc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrokxgzo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqiqudvc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3knfmrlrc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbtseeyo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3spwpmtqh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iseisnon.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vvqhgsxu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3btokxiun.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pyncnhkx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ovhifaqq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fngsjxae.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ccjrgiyl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qajlogmu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rwqeychr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nzkyxsot.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jlvzsvam.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3paucqqha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fghilyza.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hbubablc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qqbiosbo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qqpcukoe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mueahpzt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mjahbwrr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zorkgqhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvgbwlmi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ibfyfqyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqwvqtwp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dnzwivhx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zhohzzmx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3irtenafm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kjmuugtv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jjlnvpfq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqjbzoup.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3szljozme.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zumabddk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zufrcche.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wwwwhelc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hqsfddam.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3boreuweu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sauzspdo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owpsvlxr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nnkdfhsa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kgujlgfw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zipwptjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3krklvaxs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3oaerdimr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3egxneqcl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ouwvjueg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qlxcadyy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dylicnep.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hyahnnro.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cyzbtefw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tzlqdmbg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fgfrhmdw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rofamucn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tjplhcty.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jofqnwbg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tcegroni.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3umvvuejz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqxdzgo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fhydreib.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fmoxkemh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dmrxwqwj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qukydodt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zhppyrvt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3emxuezrj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcalykpl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbwelxxt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ncaxjulw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iqfqgonv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjcgjxko.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdwwbelt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrewcwlf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3artydfuk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3etqwyjlv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrlzswpp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrwogjpv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ivtkxsxw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdtxxuje.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otvqgugl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3neomtrms.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dhazqlsc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ewjohdyo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tsjsxqjg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3khopeiep.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gojzguug.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3okmcdpht.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qfwupxoq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rxqntcgz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3srwkojjp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rlrcdcwm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bjbltlqk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hoosqrta.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3harghfnp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3evenrozp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ccucmqrj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3feurzfge.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mooxqbnx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qofiqlna.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kksjzqxx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zffqinhd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jshtnyrh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3symqbkyr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nhiiistt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzowzmsr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kchtrtzh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jnlznpgu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rebsaunk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wreqlcbo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmchnsyw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3scfxtyep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcafcpfs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxbseqmh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xkhrumon.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gybvxdoy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouiyynun.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjwqqwxd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gqllfrhp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbcfezqo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yyxdrwuu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bicayhxl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgkwpazd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sguooqan.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gswctwbc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3labolowc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3saohqnuq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ugdexyhr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ctuovcio.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vodlqenb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3awgngrmp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ahsmdwqf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ylecoyqu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ybrhsgwn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3iarlvazf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3eipctwir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ximgtjtr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3eojsegjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbncqksx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3auouolxc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yszwnfrc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pdcjhtii.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkjbvefq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgpsunql.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kctlgkpa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3umfomfuu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3omyzvkag.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3akxfbkwf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ezmsdbuy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qbwccsvj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlopnfar.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdjluvn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lckhndmo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vyraeusx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3biihozzf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tpbgjxdm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grlpztab.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xirczrwp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oeqxjeet.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vwtdizvl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vnaqirco.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zkjybyed.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3copifysx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ulwehxjd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ngcjwphv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jqcuolig.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3yhcaikla.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3znzntase.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kjdtctdr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wzjhzsag.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcrucvao.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3faoyehyc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kwudzffh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3npjqntuq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fjyduoyp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3enydamfl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qaogoggy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjqmmgjr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3flaivrpz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ykxgtklm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3daypzexl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pzyhtofu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tkzafxcx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3aafmztyq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pdecbnga.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jzagwyqa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wogshgdb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3alwqldcl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mixwbadp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ulkvtcgx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ggtjiosv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rohigowr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3veywtnak.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ozjaknpn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ovjazjzv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3apsvkeuq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3trlvefgr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3egyijquz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3febzmlvk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jbpuuant.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3enlgtrsk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aglhhahq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qdtdfmag.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3daciobzb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3erodewyx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cirplzgn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rglpocrc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lqphwkgk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3udtbnpaz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dnsxxyti.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3illvcnsh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yyabgkmr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3goiebosy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3aksqtxxz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kbqtoviw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcppdsqs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpyafreh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ubxycbxt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzpusgif.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnlsfvix.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jjhlmjrn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kvtdjors.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pxjnhlwh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3smoyquel.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ezghmgiw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ktowjpzf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gostusoi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mxryvzef.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3driemvup.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3msvfhtxx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cpegcerl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxlzytjv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bvyhbqmm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnoaqxns.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ururteyf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pnqttrxr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ralayndn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hgzzfwvh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3aglgkhou.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kwzxhtcd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjkifxfi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pikuleaj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cmxfgrfp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onstdiry.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dsthqseu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3veycpdwu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mvsbjsrq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kikrzfhi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tdxlnayu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wosrurxv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uevjvted.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vzvxvfcp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kpaichxt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nixrmnsw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rclqzpqm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tqruyvdd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zecgcndt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wmvattpg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mhpwmnds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jghdwjcu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nsgxyyci.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hkpinlpa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rfcmykyb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rvonfrxv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ceihwxlb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hnbcqdsg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3boghuijo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmnlspre.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3budppber.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3elpzaxrg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3utrrlzvw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hhtqregy.html


<!-- 参考信息 -->