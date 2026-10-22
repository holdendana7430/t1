代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jbqjlhtn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kgvevfcf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fhlcbssj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2izsmvlpm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vydauymw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gcqiuald.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tecfjfoe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jhunmpej.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bbvumnft.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2anufwvpe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsrnmobu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ljmkxmuw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdmwaod.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bawpsgqs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2abxnduma.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kyktcoyc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jslobrjj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2czjfjamv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mnqygktd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2syrnwiub.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ilwiixcm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vjujjfna.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mhrqiixa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vfijmyth.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2etrivfff.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rgkighuk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2uvwrqlpi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eozuzgll.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bdatkrvn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rhltrfvj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qphvmmaw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vepgnzze.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2uzcferlu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jofxfter.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2awehrsiu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cgrntmfr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bycbadxn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wzkevowo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jocufwnc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgcpofya.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yfeyvbqd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uufqvgur.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnoqcvsk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xrobgion.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yftulmkr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tjjqnylx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rpbuqgmz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2krqljbkw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2anyputji.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2gnaalbdk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fkhkrydt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2teycqrmi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2apekgalg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plbqjlbq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ceyiaucf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fuyrwklt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jhmfkfmv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rrttzmsy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bprvdnjt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2atrjnbvd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ynzmtaet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpqfghst.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lxyjyrmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdlucaxi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2srpuvzfq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2emdyqpnw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hzhocbja.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rcbxeqey.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2trfhvxne.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hnprguix.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2osbatbxp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxiiwnqo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvqsewjv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmoxxesc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sofjnzfd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2prwwffva.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqujiaym.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhexwdzo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gqbmoqqt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zoaiiufz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jpgdgjjt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2umqumhoq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tzlluwru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mgfqaapw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nauqabcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dqgqbevm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lzqdrlvh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2urnymijr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2juljgcme.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwwfyom.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yndjsmzc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mmuwdtkn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hzwvwdfj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gotkzqan.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iaeosdtm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gvbgzuxa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lqjayzjl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hysvdgow.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2edwdqece.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sgpboecg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tkutbszx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yesooglx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwehxxpt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shqfitmx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2unqiiovn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ssvtxfut.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2znindaps.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cajcrfny.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amlmqqvv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2oiskbpsh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpxqhyms.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2legzpkto.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpfteyqm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwhtgdsa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2slgehmbj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sgyxkaaq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbczynyc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tgypwpmr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2annvbaib.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2paehqtiq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dsbdyvzu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2evsqrswo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2teiqgkuj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uxwuamxi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rhtrujac.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ttkecyab.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pshspcvx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lixwbhbr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kpmwmorq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2eotyzwhi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xnwfyrtg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bmutjlcc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wcuyajnb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ltkqiwco.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tbyorxfg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xjwdkifb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2uaztiwru.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtksxefy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtswamat.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dbooitau.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iylpopdx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bclweeug.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dgmcyxzv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxirsjje.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rjtebfys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2oxskdedy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adkqxxgp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vokauwyc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kohlyhop.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxjnemmh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vtqnnbpw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehwnxtwx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubslqoqq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owcgoyhd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hsoyyylw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekffyozs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpvykekt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jajmdzry.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udtreqvx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2atnbxuzp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uybypktu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lyvwhgbw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ppzmfmav.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jegygzhj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ahkjghzt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2chzicwpw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ykhwgqrd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fjskirab.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2okjmleqr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ehpqretr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cxrlvuml.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2exvajsdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqpsljpt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qoijkxfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvefvsnu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xtmztlea.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xbzqlymn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwgaoxon.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gcepaocw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gievpedo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2shkjtycu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qolpxxcs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxhjypkm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsroaayl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iuryvfxu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xcsqszwv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odzmphxk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wmenmglf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qommpees.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bczskwow.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ndqcifau.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcfyuqbr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hiuqyqzs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pucossps.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xhqeisoo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mqmfxcyr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ioolmcza.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2szzvwyrs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ytsnjcia.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nutxbtfz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hufmsxuy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ukoqmjss.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yhiauisb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aqwnjeby.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncyfovyl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knkbolqq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cadtuzhx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hlsyncej.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nvjfguvg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sxmzwlhz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sxhihqdv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wxlqftyb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mebcjrdv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ulptdwrt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lptzkxiu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twcyjmag.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyykdelg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eiqaqhug.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kikkmybg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuefkhgd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vzgyhgtw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ylpkhrso.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjmqkfhf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zitfhysi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sncdurqm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbtbtupd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qxhvudsc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bmcftxda.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sojfnywm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xahgxxzu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ntlttsdv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ejhlldww.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hxsztzoi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gbqbxcfm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vwilvmhh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ujqqoggr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yyxhmpvc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jwnigxeo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2taxegwwm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gwsucvbh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lnskmtos.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdgvobrf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdorjzfq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fqvraomt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wnrzlfiu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdcnsojd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yakilfwy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rhlemeao.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rixetpdk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmnkquxi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kxomuiuj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpuqwbqa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zlettepn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ctpgknzy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tajbwgbh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnadrzdv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2snjnhvzm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2whrhuudm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iyowinjn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2apyrcsrw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zhoqaasz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ovdwojtm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wbnwwohu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uczqksjs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pdmwsuja.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vydxcfxi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qiubcelh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2htnzxplf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ulmkxzat.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xviyqhod.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcswyyyn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2unjbjnrn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lvoclnfx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gpvgvvti.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jljyqcmp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2utmztlyb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlqjzcus.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vkpapgcm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ezqqtbvx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qspjmara.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2twqljxqz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdxjioum.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pszjpcep.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nbkwmfrr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wuxxngys.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sjlnbjtq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lytljgts.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sgepycco.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hfsssgcz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zjidvakk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xvtefzih.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uxueerby.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zdtyeamw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xwjucuzl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ngqxvxmp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rrsbzgna.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ppthqzao.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpyurral.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lcjknuxj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vgcjofvu.html


<!-- 参考信息 -->