代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gqqoiqxd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lhvxdfyw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uopwxqgp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ronicdqn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2calfetqg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2njscvtpg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hlqdztha.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jlotbubl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ogxyuoxi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qjffqkdc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kdvjfhpi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qefoilsw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2agkykzev.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2migvjllp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2csytcono.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zcundiuk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jtapofoy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qzqedqaq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wkhzuzhg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bdxtvfsg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ruwzssiv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vgzzjqci.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jxysqhml.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bhqabvig.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wkxahxdm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gpcbtljd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ttclwjnf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bzdrbnzh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fpfxlacg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mucpfitl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rfzsgvoq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2birfcttn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcqxfbav.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2oejkbeek.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apdacsqd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rtmhbqfp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qteeuiqd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dibahamz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kkfptxqd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tockxgrp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2foymympl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kvwyutgq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vptbcpep.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ctrwsmjm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mewclxbf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfjklhi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bxacdzkv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vexbnfln.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qweeozwq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ksplhtxj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yxjfqbdi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xmkskdju.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bdopfzdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbrxihos.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vlaxhmap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwlibuap.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dsxxawqw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dfabxdec.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsewqcae.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lradlwad.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2booiziwb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ctfkswrf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xralujai.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvatjjjn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yfnjfhos.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wkzibeps.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pzjqepyn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfgnqxvt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pwkpukcu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vprcqsrt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jfdezzwx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qosybdey.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2aqjaktuq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2lrsgfvix.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2fjurwhgv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gezdkkzk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2phxmtmam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wjfohdsg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2liojehwm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cimubtfn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ygumquyv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gvqszbpj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2apkgjqtn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dewadgms.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2glrzlaez.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rsibjygz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zjxejxcs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rczeuznl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rqhkaonc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bzbgmbsj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yqqxmypp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2seflckgg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gnmdkpns.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pnczvldr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ubmlpjvn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehvaklsy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujpbnjit.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wsinqbmz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xuoveglb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2inmyuhhl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gllbydrx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2melgvmxk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwvrjyqz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tupkgrvm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfkmotjd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpjwtpxr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zyvwzufn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlskylgt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yaehpdaa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrewftjz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fipgofec.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qduwewbf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ujpxtztx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vtrcplsh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dncacvig.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rhtcntus.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pclopypn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mdqoftlo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cmdvdpvr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rhkpjhwn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zzgugxca.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2iobjspgw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bgvjzela.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bjidqajj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wiflausj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mamcjtsq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pfdrvivj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2thkjigup.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qislevsc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idooyexg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxolinit.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mqlljhfv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ziegvekg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bjznetol.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2krzmxckm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikygeuae.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lnumrqfq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2oobafjub.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttopbdji.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yhzdfduq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxbyldto.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrtdasit.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fzqduoqa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftonwtrj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzcrpbuf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hedlzecm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hasdeqjr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjexsygq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yxyvncgh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uoklzbvq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkhxhgjz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wmgxprad.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2txahbnud.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgshqqid.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2oexcoxzj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tinznqqs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ikgjyzfk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kxyrnkla.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mhcgzrza.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yotiwcek.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kdhlpksj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2scsxbpfm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dprqjuso.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2blcfoqxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whdvppyi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qopvcqkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asndoknu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vddnhppv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vrygvorg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2druvofsb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2svmpbgzk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ekvmkkvx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejtffipy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2iekwcuri.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ablmwdwj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nnzzjzbl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yufzryyv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ebwkuyys.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srxqcrww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oinharvw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dfcywkth.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jqebphif.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qprlaqtx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jwwrqrid.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2afkxsjix.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bodmzkab.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eymrznvh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2evyogxno.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kldoymfj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mzhnyddt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xsyloqdk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tmkbpmhh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iyjgcpvo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jpzllotb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2joxkhlzb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tstdvnre.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2paozfoum.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbpaqvda.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cvmbizjs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsktcmmy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yjjqrtqq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zzclobiw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eujvkkys.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2btopzyab.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2smuacwwo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qvbhkwyy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jxhdcvwr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zooehxcs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssbmmbip.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2elaudqqq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vybwlqtw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zvdjsdna.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2psexagqd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rhqldtjr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhavafnv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wdavqgue.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yufmotnd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpmkccij.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nljgsjsz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dexsnpgi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bhbocgxr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dpzwvwar.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ofwzwxqy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tepsehpo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hfdkwymd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xtoymzey.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kzffmssq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2yqickraz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bgsalsww.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dxctrldv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2umlcitkp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2opkgwwwn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpqeyqto.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zisvjmic.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwkttkln.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2upmhtorj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rpckvwst.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wmwbetjj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gptcqmwr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2njyyokig.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2igsyjzlr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2obtvsyrv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nmzqgmsp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgfbjyey.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgdcskay.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wvmohncq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2aqbslrci.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwsyxaur.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hxlposcq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nyrpvqdt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pmgpxrph.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2drwdwrlo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2haotiglo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tyofiguj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pqfhugkw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gstaelth.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gykfdzyo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lypxpnvf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2iofevitw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tkajesco.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wnlqjmub.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2elajaoub.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaexopvx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cucncqqb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qsqaxljr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tspvmgxc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wwdhctxg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nnfmumro.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzpwrsgz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysdgkose.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ottxcose.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wpotpaig.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uleuucyj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2heppzyao.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vtdfdtyk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mhztwmhl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pjskrgem.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nlwmeqeb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ckikzqgy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2imvcqfwl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ippaylsx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2esmiisci.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pqxqtojx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hymaxztg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kmtxyioy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qjzoqlbs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2efhppuev.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dzpxxrye.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lbiavkmz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wswkayih.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rwerpjpu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lxhdwqhb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oapuvxpx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ipcgqlhq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzklexmc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qihbaern.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gwvmyydy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2psiuqezn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fmixxhtj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hxnirlrs.html


<!-- 参考信息 -->