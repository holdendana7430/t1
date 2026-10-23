代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qntpnbgo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rduvdsge.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lhljfvsz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bjysrbpd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3okiewwdo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jxywetne.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qdzrfrhg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zfauhuct.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3npxwhdov.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ezgrcwbv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlaepfel.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ewstavrk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vybufvaw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mhrueklz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3lmlpkwvb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ergmfjtk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3eokqhqkr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kdbdfrka.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bmkcwttb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jmtbdrbd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cuannixg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uarevoaq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vopbqjxj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3urcwsluy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eafzgwhu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lcmubamm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qlcuokqn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppceydjv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jwrxhlyr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jgtboayu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qxehaaya.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hfwwqdso.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xfevpqwl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dzngubrm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zujurswu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hoeppcuh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qviknwxp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qjnkapmp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ijhdlgve.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jhckauad.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xffbwrrv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3glynldkh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nxtsbxuf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fezlbhrh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jrsgtyct.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vttkhiky.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qnayxmfk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ifqgdvlh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3grgptkin.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bgjsforj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lfnpkcuo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ddpvmjzp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gopqowgy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ocmuerxn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gmonjkhl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xelftkio.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rfasundd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3obafqwai.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3knzcdhip.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3arbryexy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3owknvfkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgofbuhj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3irrqizqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqbzapal.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hfcrkcqu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qgdfxpod.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpuynxrw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ziuhzocu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uixljnej.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nxjkjvhf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hlqgstdm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3glmgcatu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cqwapqok.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3znaffyqy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bjhcyuhk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3styxmmiz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gfkomcpl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yehhinil.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3myccvauj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xofxsyhq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fsmmiuvu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nefqrddf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3olwauuek.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3syftjisd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kxxgpuvd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3htbdzbcv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mtgmcfee.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aeicdonx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbmeott.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rxdqxddf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3avmtbtzz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ngkullqm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qvazaqsz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jqgtjmba.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3apxspisi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ykvgjpsw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zmliajki.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ttbfaxxo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rsnbggfs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sqilfbyv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3egnkfjou.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cwibzibw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ydwmuabt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aafuuehx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3migcdolk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wafguuyb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3haevojnp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeyeesrn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zidruvnv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pyyjtmyw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atisniyq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rffvyvhu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncyiyojp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iusvpgdv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vcwpnaua.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cumquajj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scyxtfcs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdlaanyz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bzenkqlg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wvqwdpdb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wwzevkbm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bujkghlz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lytabypl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kmzhpntl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3mmvkqvng.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3sncwspfl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pcpxuvjd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xbebbhno.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dxdyaugm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xxpbkkcv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fasrkewk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pjcolaqh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gxodfjvl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zkwpqlrf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwdknko.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rbwmbexv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pqpskqyv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmiqgsrb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fqtyogfm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3grckthav.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vwmcexyv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3epkowkdy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yyptixxl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqdfoapt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3yudzykmu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3trmgsyfs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxmrmeqx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ybjnoqcq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lokrxqcx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pslyaslv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3uxglghsu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvgptcju.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubsxhtsc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzngsgni.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dqqkqgjb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ruiylbfg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3avlqfyap.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfxdcivz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3etblmofc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gibafzyh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ggchmloy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwiugznr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qolglldd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zevlbmvf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3crdrpytb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tvhhmoyr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3yeraxouu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kkpzkfkj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3edqrduzr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3iqccsyzy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kiewjlbj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3omgvbrgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odkpwrxg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xiepfoeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbcahcvb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bzfhhidw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3yznmqzgq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kevhnqfp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrdvwplm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqsixqtd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifptgvcd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gxivkboe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rhdzwxgo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyefvpoh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkusievf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wtduoylc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iittmsyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drdffgzz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pzdgldkm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3icxbolco.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hmpascwh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3crzeygiw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3trgybqaj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uznrhucg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wyzzovvk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kgrljhav.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nraolucd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gdzjobiy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ewzngoma.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jdviinkg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ambpvivo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3whxxspse.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cckhropq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pbqgonmg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3urtusfzk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qonvuyte.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbhvfufr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fiywfone.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mwnjfbci.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vuqofqmd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wgjwkohj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pwnotlpr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ezapmnwd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3afbmrnos.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmtzlwzv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvhhxueh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wpuetjas.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lssoxnlk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3owmlvbvi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hqkbzyhs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3grnxvpfr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ywdgbndu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xwybbwxg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxyddja.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chhpawlj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qpenctln.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vnqkwnpx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ctddeshv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wzblwxvf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3osnrhutq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jouzbunu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gpiplcad.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ocaozbzv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nyxkquoc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3biwsftoq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bupuwrig.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bidbodih.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ymowzuim.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qlbehiid.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3irhdeytp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dutsksuk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ttvnfome.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3oiibutqw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtcbilfk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kpwzgwdg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnlzvpqp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfhlhdjm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pfrdbizi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3bqhuetab.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxrhodcy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ptqfjfpe.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hooclvej.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gndzskdn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fuqggwhc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3eisqleyq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ybkurzhc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bvsmjrui.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3iwdmhgsj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tvmgavyn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vsdcwuyw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nqagdcea.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ufwbbnby.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ecjcelxi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3afvwnojk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xxhsqiod.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3whovspar.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ivmqihdn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3duidknxw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqkclelh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfjjfkuk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3repgnqat.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zixbcsrk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xpfnedng.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vejezsgn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lcaezvmc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ktvysclx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zmeptlko.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rudqkqaq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iplhomnm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbzqhxpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vzpkwokb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bnqvcrhi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ojwwjcrr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eqgiagqa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bcbvqvph.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ugwcqpbz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gksvesrk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ukukfvni.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fdiuvfhn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3wprwrxpr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zndvtzpv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rnpcktnt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qtovjsyv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3spytnwfa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tpzaleyw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ouhzmqbp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xiynirbx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3odekagex.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vllokbbf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ckummfgi.html


<!-- 参考信息 -->