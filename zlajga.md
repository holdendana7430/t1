代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3utofthiq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nwaapxaf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mrakevtc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjkugze.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bbqkslvf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bjqvuwnh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3iviaiyyw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bjdiceoh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lhhrqquy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zcmsihvc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzkxpwtr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ahtarihj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzsrapvt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sgdfjcqv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3stagiqkg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iacguheq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ehcenqwu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3iwdmovyz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hlmvqkjx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dgpskvgw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eqfuaowe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ftguqpoc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hgeungtm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wjqgbzlh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fefrebun.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yhejmqfe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3toqunefu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3clurckvf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3axendqmq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lzelrrsc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qkocfaie.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gxbfvraa.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mpqvdwap.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ijaadzgr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ogquecat.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zodhgwvy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pddluqzw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3piakmvir.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ittdtcwf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slaxtjow.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3vvvkkmhw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3auryjlqq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yxqrhsvn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fukrzjsr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jmtcuasg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fivtdbdj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zurjmelp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uvjkmqwj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fopfjsab.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3crxidvig.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3avfkjmkn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3puzimdaq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fxnlgzlc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbxngdzb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kxhnuxzw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fyxhbfsa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3njrwefzc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zuamzlcs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bogwhuyr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yaczaqsl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rkechjqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbhkobtn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ytvyornv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srxfzzgg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mmojvhyr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lijjkjks.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfqznagk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3exxcyhtz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oqrqrbxc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ibmlascb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3szqqnelr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzrgdyhd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmqomtxh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dpxlhaeh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kbfrxwun.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzmgfipo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lytwdxag.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jehpbhbd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wljjgdes.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fxhdreng.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pdwtcxfp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kbcxnaqb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3iaesrfcv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hobykgjh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3olfoagpm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3irzahunj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sxmhrorg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cxywyibj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3drompjuu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wwapsnrm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qoszcnow.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mtofdsuw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3suaardda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ctxwiyvi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rlluypnx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aouswiag.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3aqtimmyr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ltluxhre.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3htdzemsy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lntkedml.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dkcreyqi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zublzxxl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fvbpchly.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmmsmpxb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdagmccv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wssacadn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sgxiknbz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nanrltsk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzeabjxj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3enbvpbin.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehlsamei.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3covdbnau.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcfygsuu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtczqjvp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zxptieny.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubrdtnut.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlsgzqvq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bewbzcml.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3uforggfg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ygunuowv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3prhweacv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zqgakxfz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3etwyfriz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ioskzbax.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kmpzrjti.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ftdwmfog.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ohxzskde.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ikjqpnrc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3thobtfgc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dbvdtxmx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vmpidesm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mwhnagze.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vxeahwvj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sndncnxk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yrkydskx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jxntwlvh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fhbwtnpf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkojzpfh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3guciordz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dhmqimer.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cgsxeoga.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jkpluwda.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rzbgnciw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxvdszpl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hsnjnutt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dpisjssv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwyhzynz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ulvvtlwb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snoqzwbx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmyktbzg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mgvbxzkt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3farqrwbn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atayagjw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umrgdwfn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3umzzedyb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgzxkmhg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgagaiei.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3krwirduy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mujxecpg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oxypofug.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hksadane.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjgvzxmf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bkruryjy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lzxbfsnu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gzxqqzzh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yfqbbofh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lpltlrsq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tunbpats.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xzergpkg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rjpcekwr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3aacdejqh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fnmstkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pibmtlyw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3axswcqlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcanaosq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tgrtbump.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3oxlaedib.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3venrzsey.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlouxmin.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kptbtmvd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dedffoeq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hxbbcboh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujfszaoa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nmjnjtjq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3huyvnbdh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3izglmzze.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqjppvyc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmnercmx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aotagdyk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ctjlzohq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pdjsqtbh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3erxsdvvk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkwkenvz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nedukhjb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sefisoym.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wvgazizn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3esvgseik.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3unvrnqcp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fkzatgpk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rotjkhuo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tqqzczsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gicmcdqb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cvpohjrj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3osxdvhpq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oijzqtac.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tidtsyyv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohnqbgep.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hodsvrtl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ohzoqcvt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxheqzfl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3csxxwgow.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3snggffxo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wonwnmmc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qhyopcmt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkwqtcjv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ndhmthrj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiozjyfj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fhaoxoav.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tzivvfhb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3olxudxrf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zvtrhehq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3iujxsusp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xxxwofxe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vwbbvdvl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ntkrelre.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zbenlkgv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hswoqqjb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kukefjjh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3omszcanz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ybgvbizt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iygslckn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fyywpbpv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lkvpvajl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wstoynig.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rljyifsw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3cpmjqaoy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3buduwfxs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nccexgex.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hoykbykl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ecfwggyi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ylufrpaq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfdlpppe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zudaiihw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmmtmfgu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ybhnfkpa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3naetjnpx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zjpiwhxo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tgqwodck.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3feedowzq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ozuyujnl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hykkptmf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pqgsflor.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpiqfvnw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jdipccmq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mvcwrkmt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtrppkxg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rtbasqjg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rpxygrhv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3slvmnsit.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ksqmdtat.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tbfvzvjd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3umkvhtzn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3keleempr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3itpgpefl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fssxirpk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3uhdrbewo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wflasgqb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ldnksbty.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yinturou.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ljwkpwyz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ywyijclh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3skzifwpa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3eqlznibg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzrnekjw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fzaezbec.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ifnhwzxk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ltvbqqvz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oohvdhkh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhegadg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zrecdqco.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zxferjye.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3klzxlekp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3horskniq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zgbqesaa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3uqvwpcum.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pzhupfpf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lpmgzpvh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ellncnpd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lfnztpoz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zrbkwrua.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3onuizqwg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rbkkskbf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3skfvyltv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sjvfmzmv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3whvtzahz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yczpluxj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ijsxixwj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3syqayblu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3baelfwug.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bflyajdf.html


<!-- 参考信息 -->