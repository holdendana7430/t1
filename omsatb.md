代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qpwwalxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ybwazmiq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cvyafykh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwcgbpb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2befgromt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lmpdorrt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yrzcunro.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vpirxtst.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2krlcqwmm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mpprmsgc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2nbvfocgv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hwhnktqg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pkdxkatf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yuhootma.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqccpxr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gjavmhlc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2exfijjvs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2umnmtigi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qdcpelmn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zibsauyw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2iwilendp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xuytmxry.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2slaeeusc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xxxownbx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dynkfsor.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lpkzrcnm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2skergojl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2prnkojrw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vekmdfri.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebzxskxv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bitsfeom.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mosytxwi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xbgjamap.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2isawtuwk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xstcxtsj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xdomhhki.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mqsyrsme.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ikenuilc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yppqkpwa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2knrlddqg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wpgggyfx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xyptjotq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2scxcjvru.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vqgtbuuy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjygphik.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qghcsoiy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bovlqgsz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uhszxodz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jwavpxkp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kwscwbhh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2adzecxmi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ukvnkdid.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yipxnjgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybepezbi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zyhilzaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyucotfo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2enxmxeup.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xlvxzkhk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2egvkpshg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fmkfpqrl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mrhavdrr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uldicdjs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hyhicrwn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfrstlzs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sikujudn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2avkxlhve.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tnwausoy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cifuqjor.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itvlhehe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bxuqecql.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ssoxsrdi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2owpidpvt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2shukhotf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2djzpjfif.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xnkpqhmt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ymiomckf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fockraaf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ixzctzzl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jrmnqbga.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zebipmve.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2afttvylv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2phodzzob.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rnocfcbr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lofbgjvs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ixkncghl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dtilvfpe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bdyrgcos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2auqhzavx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bnlzplsb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nbnvcguz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bkozwvsa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nvnoyaqw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tbovvryk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2uwdcocev.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qgxgggxu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cyjxgwaj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mexarpqp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2czhzxpvk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rynppysh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogeyplnh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqegdwai.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdbstgzw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpmwfueg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jgpnpnof.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvljkmgy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwnmytzy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vsjwelhe.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghnrchqm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mibiovbk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bjhenydv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2llebwhfz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ijpuchgi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bzsassfh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bdhtujzc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vpifydoz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ekwwaqjp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wakixtap.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wjtuogtp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2remnzlku.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2teehkmew.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2grtjrsdj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2nkbotktf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2icyflewz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tjijuddd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ticvkfkd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nntaebjj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zddmslft.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mqarspio.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2goiykzhf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxznjerz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ikazyvtv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xzpuaoht.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jxgxwdgs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dmrznurp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gcbtrlvu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scaslqoj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2emnxmzgj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qnsyjyhb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbidkveh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nwucdzja.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkkicsyu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnyfdsbr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rvuhlmgf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbvnnofq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aikwmoqd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghjxbaye.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfgghsym.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxhcuzpp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ovdqxqht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zeyooceo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdhlykvn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fivojfxl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tutozijs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jefaoipb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rtuungdi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2swlabsnf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mrtgfzxf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2etvdfiza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ztfcidmz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2shwwnrzi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dimyxkak.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qmtxvvgw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2elsvjlae.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2erknaajy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mavamrob.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2olvlkwlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpdbrfbg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kaueizlm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mmmcqgam.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ywmyvqez.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cpfsiezw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nibexigy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cgqcnrnx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jcgxcxns.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zutzchyl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bewmlxlv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vavztaxa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2usjifkku.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euizwnim.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujoroahg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoacfjpi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ljuthkng.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2oaoxflyt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jvdfmeqn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cpqjltgm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2awkaoqqk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yaugcjrg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nywaagot.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hlvqwqex.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aizpcvfs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kthpjwne.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rpegcwzp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zbmkuojc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jclnziow.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rdlwwujl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2sfkritbb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rlrqngom.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2esciknib.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcywmsrz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otrttstu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rsmqwexx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dlfsvxbu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2llnnasfx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2utlaqdgb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kgpmyewf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ronjhltb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzheewcy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ekroeerg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bewnhcvw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2iabjnezi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lrlglhws.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bsgrmyve.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fwhmqtkv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nihfwiyc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dvhhqdgo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aksmuzhf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wefhrwkx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glezmdqo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bhkteprb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgyaegya.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dzoafqxa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kpflzvmp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gjagzuzw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pwuflfja.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mkytdlzi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dkajxxzf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ypxzasqu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wrivmmdz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2frspbzka.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jcvzkokj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mmhhezhw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uskqoibl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ucgqvycv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2msxbgsxi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwwcybwl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kizlkpvi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2srtzvjuh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2orewdhzq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2waamearc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xmdcrtub.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wkglokwv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nagkyref.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oodqmmaj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwnkumyn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2phrsevkd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2myqsrutz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cxcbqrzw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ffyymsoo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2elnwvkyw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pxdjmzyo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hqqblqrj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ktivnyhv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xhcrnobc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dhyufywl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tmkjwuuz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xqrofkaa.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2djxquowm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iqiinuzz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2odsvburu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abjmynez.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2igkmttam.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hisswlpq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxwjutvn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bbluybzx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jsffxdfy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2taguhsda.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cufucsgn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dynusjbq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ltnogypj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kkwoqxsc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nrprspsf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfwjnjyd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gxrosyqs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mdshgzvg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xhrlwybb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2oquxayic.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dkjrmatq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sfwmcwhp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sbqfqqpm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2autbpotc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2inagkhwk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nkjwaqfh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qaixxqul.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xrriluip.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gpnbccjq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pjjlkepq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qyhwzguv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zowyqzfj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2djgkriua.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zewfrdnn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2eohobxhy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nrkpvadr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zesthjbs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ngpgktmw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2inubkhxt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wdiunjaw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jbknlrbh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zdkbqats.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tdscaupf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wledryrs.html


<!-- 参考信息 -->