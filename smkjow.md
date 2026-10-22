代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fojbkwtd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hccilqtb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2guaqpwfy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kflyjyql.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jltuswcz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqfrpvqb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uaiyuvyi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fokkpoby.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzcufplk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ticgkyji.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lfypabyt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qwnqqvxx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ccpkiade.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ubqgnlat.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cvavgtid.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rbldwttf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iyhhgwng.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2anwyuees.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rohuqegx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mddzslrf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rsxdhojv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jqvyhfht.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2lewzvqzm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2beyhclxg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pmalfglb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cajcvyzb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2guehrlmv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2lmjmgihd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xbvldxvt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2urbndtod.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jhstrcae.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mxsthnyj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hiiiqjmz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsnkepuj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjzddrko.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2bwppisan.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lzrhaqam.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jjfjuzrf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbbuklez.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2lgzgsnuy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2siovsnup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gitumbwd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqaibfwt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mzyhjzxd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kqnwllff.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2afkivlka.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rdujtdot.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nhymjewc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tvrmahgr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2esyqqpse.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2crpntbuz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kmmajauo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zmzobjsj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ykpcgoln.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ctdwpyai.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ncnngvmn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2crkueqbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vskpweac.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mhvawggv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmbowhht.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bknidylf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nxkqwxir.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ergtzqrt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2knliumwn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wdwaaknn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gfxavgoy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2esauxwgy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shfrfnou.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zpwqoitt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ngdnifqx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2knmkedin.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rozxdngj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxnmiekg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vzxczain.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2huthoiqf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vpbejezz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nqmoersk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxxaskrr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uefvoste.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jhgrpuia.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yoezeeiz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2thfqnxll.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hchmjwtw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qaoenaur.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ivujrlax.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2amzjvhvc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hnjcfgee.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ahytitrt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2busimmvf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zvhoqtkg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jqihptzu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eyggwzxl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lobrjmzx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eefbbdpi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2knhjirqf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bxelojwm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uzegignt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ytyqfsob.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2blnvxhjm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvyywqif.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2muclchhz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qajguegx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yzwoigat.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnrqoxxh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jteythbz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrigop.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgljaslu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qimkhdbs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upyydscd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxxvnpii.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2agxttlrj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igjvbidb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flvaxfzc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mxqrnirp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ubnnryve.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wiacopya.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2szuaplpk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hudmpsev.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ihxseowz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqpohfqf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pfejytrk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2licrinll.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fityfyqh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lkqkvkue.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kictffqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dannxsiy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qrlqvxjk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pfgolmyq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ryjhslua.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dotzexuh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zctvqmof.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rxarhbdg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ppfvythx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxteigae.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vygaluuh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wjwricdv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wwkoawky.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ihgqfmoo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fityiagx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgzpdszq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2inesfwqh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2opdvkbrq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wiwxvego.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2veoxuqpa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpcgbgsd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzkerptx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cmewqrdc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvabqgxg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2debxzmqt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzrwvhrp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dqtltxzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmworgdm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihzrufxw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2muwnrark.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdzkavde.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yqzoopjx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2deugnxro.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsgywsop.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lywbanpw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2opgbrkij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2miismrya.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2qysfmllp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ehvcnosj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ljcrkxun.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zblsygot.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2torxsbce.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2znjismpr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lrkvauxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edgxjgyr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2eymjvmsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fiwzsefc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ffgcdvyg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vxgcriha.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdahyxhu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvuistyd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pvbghhob.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jyhnqqre.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2omgqlcto.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2juphgovy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiuryvhv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2azyiuflt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2msyymxbr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bvckpznk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bioekbhz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpzfsdfx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cempzxnu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rqbgbnbd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kausphdt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2scnvtqss.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nicvcjvt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nqapwiwx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qcsfuvaq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uniqpkcp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kdiovgrc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lpplarlo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lbmztixt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fdvlxuht.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zzsffnga.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pnsqxlpt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2giowhuvv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cqldevjb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhxzyzhh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gggypnti.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mtuezlkt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yunvspjs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwtrleuu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ywfikflr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jafugbub.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bszepeaz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xmkckbzn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hmrzqafx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2elnotpbd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aqqoqoht.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hhirucfa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zgdmejfs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2euyfxxoa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ixhorlax.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2elnprfar.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mrsrhyqt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lbqqdxfb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpioufkq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fuzmlinp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xvyiqpwi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uznnvqtq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jxonvkfj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wauvowff.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fsadnnmt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dvqvkdht.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2slxgxtds.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kpaohwkv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zliwhcao.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2oxnrrbjt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qyztusme.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2eittuvyg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iyuwshlf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pqavwslb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ijnaeabl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2szqzqsun.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qplyzxrt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtixudha.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zkgxunlg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfrtzacn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrxssaun.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zgbcgola.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uaykqecl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uagkisbs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hjuvytco.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcmpnglj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmbnbcet.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lrafunoe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ypbtlmts.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dbbrjmmp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2frcunula.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2espvpgyb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gqyfonqj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vyhjnyja.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jywodfjq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xvsoalno.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2adwxnijf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eorrffph.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2yjzghwny.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jtnrwtxm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gadvauzp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jfrstfll.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2shsajome.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pklmhbqi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pbmervmq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qjtrtbms.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2buleoecz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctpafjim.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hbwafatj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2doqzwuio.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmvgagdl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ugeszhla.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kezgqozl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2klfkugqa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yzhiiykj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ghuqozxh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dgvhkbds.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2lxohpbhh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2akulyahy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tmhpzzsh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mmdogplv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gbvwpqma.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hqpiymph.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hiomdofq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2mwbdjkcw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qdspkyzj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2djzgptgo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xzdsfhem.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2szrerhbq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jfytqouz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fqdwzbyl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rsfmxqsn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2sbldxgaq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yvpmarfa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2iyxjqmrx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fabqkaiu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqgnygui.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvefubjd.html


<!-- 参考信息 -->