代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2sgrtvgfm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qyiwyehm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ladhsixq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2syskaadc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2iozbzwlx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tqfxzuib.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rsdhxzdk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ltykzwvg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2igmewjxw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bdiujsgr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uiamwvuu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yqsipbsa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mjhxtlye.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nbyiwdkj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nrhipfzk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hoeeknno.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kanljaew.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dgzpcqfu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rvxcrwyz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2chapyemk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gsfgxmjr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vbbwlnbe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2prcravwk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2emxjygoy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mwbjumbe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2jhfpfcij.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2zrbzmgwr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2axyfooao.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yaauvhep.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ojqaiaeh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbwilutw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jpjbosrk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qehwgyjb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xahgsxrm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wgqlqkim.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ljwtpbqb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2phtpekgj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kkhjnunu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwnnmxun.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rprusetr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2brrrqyrx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fhryvqts.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwcuyaio.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ckvkmpcq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fkdhppiw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ccbtahsz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kxfwtkdg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yqgmkzkl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gqqllupk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fqumnkkx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lsarekka.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qzbzpuuw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vmtwttcy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nbgszrjf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xbattrbg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tqdexrng.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2puzovioa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ulsiovay.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kbogpgte.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2brnuzvwm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wskzitrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulblkuvx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hjgefgpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcgedlfh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cqajswxs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2iadofzsd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bsnjcvui.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2efsuftfh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jbdpzqpu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yzepyghc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ehjjpnop.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2guqoiosl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wjvwgtbe.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfyhtmfx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rjocobcn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bfwnydjr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzadinbo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxpggknc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qhczfiuc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2icliikfd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mmtsmcqk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuzcfyfz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2borahcmq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fokmzqfy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pbnbixjg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zuxdvedt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2goqfgiek.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2igrdgtef.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jasjxgog.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tlathntr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qzsndvcg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2westvdvc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xbkfqfva.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2iohqykwd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rwtkwrpd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2spvojvob.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xxqjcbip.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ecipqwwb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2peairnpy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uudlycau.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rcvrundq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fkwbqwhq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cmbjknux.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vhjhqtjv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwmajspu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rouvqpeq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyyefwx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyfhcpqk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbgiikln.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wtcdpmvm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ukyznuan.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jqxwvrfb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fonsmxph.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzfjauga.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uswmgdld.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ikfozpad.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wndzczju.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xuoblgtq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cogelfkw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iutslgdj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2fwpjwueu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ytyljkwe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2csoqgpqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eeyurxzc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ivzrddvy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nmcgowjs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hxmalsfi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2iwdisprm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2khhlzfoi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ztbaejhw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2klnissmc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xifaylbe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wsqjtytf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fgoevtlf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xmyijtli.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2olzxtccr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ddphwufi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kclocgxu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgumihcm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ixazllpw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fbxxkyxx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ytakkhkp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cakezhld.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yphpyhwj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2agxlqyxw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qccqutpq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfknyjxm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sprrohad.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amxyksbj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqvmeyou.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vwpdrphv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucmcvcxo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edflewho.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orueaaty.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dcxfjcbr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odwlitok.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2yueklrvr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkkdrsgs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljmeqnqu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rzxczmhf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zyjioway.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwiszwip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mwcnalju.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2guffzqmw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2aalpokli.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2plsugadv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fyaeawsn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2phmfbxxc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zlofjxsu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rtsuqphu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oenzlncu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2epdeewje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gyypegau.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nceqiwzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyzrbfau.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tphgdufz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kstjxaiq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2byizajkf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eowclcgk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rnqpxkld.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihftsqrj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qxcnfavb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2khzhcgbj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2smcqsbfp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2auvpmpnb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qwbpiuug.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qzcomjky.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2psvsmowb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwhuqvoz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vrlsnavx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gwlcmdwa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xjlyshzz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzcvbbyr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nfgfswzn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pfqexrze.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nedaavnd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nlmdrytn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2krcnmgrq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2okumilah.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2blvdgssi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jrucdwpr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ifkdjvhb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2adojsmza.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xonsfqlf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htlbjplp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cnfgyeua.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sivnpaty.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpyrldta.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ycctwudb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2iujxaobv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oasqitpa.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xwfqjsrs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ieoffgqw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cilmreip.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryrfyzkr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lpfrrzkr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggfkjpsr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xxlszceh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2czputbps.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmohxbof.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tbfhbafr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tadzaxtg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfcvujcg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzrkhtsn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fgklfazx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jlklfmtt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wonytpde.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdngcznz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gcnhjavt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cjkgepyn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ymralxkd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2egalryrz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oxdsmobu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aahrphtf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eyxbuujf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vfwxmtxy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qurzuhpj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cxyaqzzj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ujppldaz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2htysoknn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2akcugber.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rkvxmibt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoaotfxj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2euhthonk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bappoqlj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qjynchoq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zbvkzlet.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2biumjmuy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rmgedolc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ocmqsrue.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zyimkfrl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehtyphjz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijdswqvp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2fltbndla.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2veqovctr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysquigap.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lajvhdcp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vykowbah.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ffwnghrm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2quibtahk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2juqvqxkn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2corpxtat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mlcdivve.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lqbugtko.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wnlrkdlo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rqegsesb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cizaaami.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwmvkrzq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfjpcfdb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unlrorpk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pdtlpuqi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2chdbuukj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hlpbdjik.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yxdudtiz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bdlifmrn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ynmfttsq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtqezlup.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fzrhlaoj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kjnqufad.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ntmqvaqo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dxgqrchm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hsoxqvxp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ndijgppj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mivnelij.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zudeuiqa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2umprpfvn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2caesnpnj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sdsjbunl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kasvvgal.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lfryjsii.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jaylfydb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dargkksr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ncomnbzg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2htoercmh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kfbaxdef.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vnhbkwyj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xotatqyg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cqsnsroo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fauazeun.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mdeffwnw.html


<!-- 参考信息 -->