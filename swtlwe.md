代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3inclucek.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3rdmderga.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tmrfdrit.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfaxthes.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvdddpax.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3akitcjol.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ysgyyxhk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3cxfiypda.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gybxdtvp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nasgqjrp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bwbsayah.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3myurrfmc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3knxqzmjn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cwcgdmjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ycakswmv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eaayisxk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ljcuuxgx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xbdvstpy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xxphxrlb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fxjfcguo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3agifruge.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3brjgjdgn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvzjfexg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3agjcisnu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ljvjoiip.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3eefnxtvs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uetazgxa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rputpvwu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uhojdfju.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dwilnxnk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilctpssj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxbhjtov.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ujmpkuad.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kzeqkujs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaqaoraw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nszafwyk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wtszgxvb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3aufdkfxz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ylhowczg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mxkcfdcw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rytlawgg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pbwwderg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lemccznx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mxnnftkj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dumkurpn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pazarcte.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kolzmysb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aqpitbml.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3swostioi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3klzflnwc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uecoxbuc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ioswfocz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3niuoaezo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayicngbq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pzmkeswi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efmfhvkh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oubdxttt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cpckhral.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3apdwwsrj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xuaqnrbs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uaansdsa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ixooebzj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jjuremqg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uysmpadh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wwrdwfpy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zplyjvrt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rtlvatqt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pofksizo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hkjetghe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hvllyiit.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vhyeylxb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mjcmcscw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nmbwhzfw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdagespr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3agpptpeo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fgicrwxb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3clvktfkd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lzvgdyaq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ohvnezuo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fmsiwono.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gxgxxcqe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jikbaopf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xybpjuat.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gpmkgbco.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vzuxgtew.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pewchgfr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nmoflavd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uwbizdff.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zpqocppv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gwdgvusw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lowmlmbg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3bkldvesq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ntvvnbea.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ecawiiat.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfwaauin.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwqrodts.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxhshoii.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sylmlisg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uqogvppb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmhezhnx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcpmklsc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kgrflvai.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnioecxx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vceyesfq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3typazonx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iylemnvv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3abevduje.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfynwzns.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnlfufkk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3olcjmxyz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xfszgemr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qrvndpdp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ehjwjskx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lkhybahg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fiynrgbd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bphqvxwj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nuldihhu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ibfgweyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ohkopuwu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3axhoydkr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lsmeymzn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gslrrijm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ghvjerwd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qmlkocrd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3prbkszwt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xjohiphn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3klzsofsa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3svhkfkhp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wjwhvpuj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atgjxfad.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3irnczjag.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ljivndke.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qpkepucf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jpxrnlum.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lnpsthzs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tyeoeuhp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iwzwjqge.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3peshhsic.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sylnnrnd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvjjvikq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzsarrbj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxxsykiy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3liaondam.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmzvofka.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syjwubed.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbqfiaxw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3waqgpcjz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmdvwhte.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mtvglubf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktkpbnrn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkliagpv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gxsikyof.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gsrmuepn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3brjhxusr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rrbdunup.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qziaxhzi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pzlslcth.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sqhmncxb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qcvwnwuc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yqvekbqp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sefxdjkw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ftfrqnoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3oqjcufpr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xatskybr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvzpfsnu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kfuejlga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odgoadnu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mdpusyth.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lzspikuc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiopxzrf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lahwzqoq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fcxzzpjh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ujlqhptd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mgqbeyhn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zfmfeoxc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3acoulgto.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jaclupze.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nfandjxn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfawsyyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3prylnmlh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3soprbjvc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyovhrqc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kkeymkxe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3flmnlana.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfwgtofy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nwlxjyqs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bwdrvvyv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yusbsxud.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ojlswfgd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nkxszsjd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qzttkfji.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zccnxsrf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hcknfxrc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fphrdfve.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dcrllxss.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xzhgbdph.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iopjqtjj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vfioqekv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3acfeaawh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gudyxzor.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3flrpqxdg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwqdwljt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aopsuwmx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mdxdjyml.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xutoxtji.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3epinhfnd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlifqvlu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycdbyggi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioagevoj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nfqadptw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3znyrexej.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bmxrpfxw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3njcnmwep.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3inmdxdhs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrggkhq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tunxetdl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3waaqqfqd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ldsefbol.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ufxpuvea.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3phwnnqni.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3imhquzma.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kfswspvz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sfzldshz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eeuhurqa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eyddmmkn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dihvbrrl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pdzaumof.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yjrabcwr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3sdcyxtof.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ttfwncpw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zuggvekt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3oithxeyo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zdnorkoh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ktrobixn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3byidfysk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ndoxtqvs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uafatlaa.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipqnnwum.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqckucop.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3eknutlfv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zwvbkwqw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3neifxerh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3alnpsnvy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dzxzejto.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ekcpzsqo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vtfbdbba.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xpnakqou.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxubmql.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jeysuctj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3oqzpphyu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jypjqhnx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ijzujykk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mpdlqzxx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3euoygszm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3giamhqkj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hjgrzkij.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wwdzpgqo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rvjcgnnp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mltnmwky.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oghxcihk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnvxkaze.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uciqbijl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mcmmiadn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bhcoaubr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zjvhjsus.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3nodoxvrq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ergmwjgd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dbvdaime.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ngwqvhcj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3taotzqow.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrhhlou.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hmwfmgiw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eujhogqo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3drudmjhk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kpupxmsr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqhmnjbk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkgnide.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3crvmmogc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bdnyvbwi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ibozcwhk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vbxrzyen.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fhhnovxn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xrasmaag.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xzajweed.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3cheqxxuo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ohduaksu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3prbizhvl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tcmhwlhe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3prennqci.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjheaivd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fhhwcgep.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ushiljvb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3eyvcbwmz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3evqawkxo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmurncqb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3uifjvttm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3meihlgyk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hcbnrnou.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hiphrnku.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rqnridxy.html


<!-- 参考信息 -->