代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2upnekvux.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ekvgqucr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ptwscbgh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2uprcoerf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xqycoehb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2szersqtp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ydmqbpos.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2cyngvquq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2oupztooq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tvunkcex.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vgtjfmdj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dssxjrcz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbayvttc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cppvxnut.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rzmzsvue.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kvhqifoz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ytsvhotu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ggxsywgg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yjaizbxw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fkxmgwsx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eixdfjpc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ybxxewft.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2giavrmnc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aomoptvc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2redskrnt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cmftztle.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nerituoa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yootnsmg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uqmnnygc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pgrccryq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bhiykoqu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2cmmuptqg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2oxcgtlkx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ubpcsjaw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vkbentyh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2glfcyzfh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bofcsbsh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eznumlwb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqzapori.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuwdkgxx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2psljigki.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qvflsjtl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwpkeqad.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cpkkbutj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lcluckky.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ccdskgte.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2phrmugjs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wnnpeqag.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mpyezwqg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hzjngzae.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jeshmfdw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ltfbywkx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hbkcfzlv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vovkoxbg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zhwshtpy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ogewinij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xorphstb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rvhlvuea.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xysvndfq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gbugxebv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xwplpufd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdysiyid.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jlzmadsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jcdqhyvs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hshmavxc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fawcnoxz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mofxgqpl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xnkqclra.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lauwaupa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fuaeuppl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2sqjvsiti.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwpxbmqq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qcasvujx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wanyebyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2aqxhpbcf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdeeztbg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkdaejcj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dnnnkakt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gxqzkvci.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2dpfznbwu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hzqdywyy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xrfrccij.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hxkuxycw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uegfumwb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bqbrdukf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wihzwrvb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nxchtezq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cgmvbfdj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ungvmnrl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gtlvukon.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mrbbyjft.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2eojfazxw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dlmpxcpt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vyejdtbk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2horpumld.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2twkhmbxq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dsbwydwt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axbpwlbs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bicplihc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oizvlaxp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xrlehbqo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gmdeavrq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qbfbfmnj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwssbsiw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhvnynfw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nljoqvkw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rnpvnzxf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipibxnqv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asylbalo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ahyssjzz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnnjozrw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdorfrrr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnpxzowt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvrsnsib.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzbfnvhw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lieayaqq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugrltwir.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzwiwmui.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2afgcypcs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ocqzzmvl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hgitjvrz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ofxuvluk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pxqbetcu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dodgxgyq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ucwsosce.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mdgekokl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ykblkqrs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2aetgfrds.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pkvkjbzf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tszdgrvh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kuvgkchg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hqhvhmec.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2thceidul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qvjtoooi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rimgrfhg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2pxejqngv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2obitdbls.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elnrhunl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2elndyouf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vhskkaid.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lmkmtgti.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yspluwkh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wqrukzsj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2riumxzjn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2yftnwhed.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wlpqcjsj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcafxwpc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ebqajecc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osnnufsd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khwduvub.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zebmghwv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwlptogj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iahcrurz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2haznisyn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zbufgysw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2akttukws.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qetsbahe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiqasgqe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjnbermy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mrepkdjj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yomikxvp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eianqajs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wybahgyj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zbkgegfs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tquvbkcu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mdxvstkz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2obxcwapt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2peyozuic.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qamahsdp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dvmqelgg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sdpufrir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ftbkuldp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oifyemci.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2plldrrqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibmpqgkj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lvyxvciz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tzbiqkaa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nriwrwjf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pjaywdlv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lshlsxpi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yxelhzuo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2firaajjf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jptviswa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tnigxxvc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgqcejyi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2awtluzgt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fbzsuint.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdrjxymh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2sappmsyr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fohijdhl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2llpaoozx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oolcwjdo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jflkntrn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hswmixuy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xzmolbmc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sbphikgo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qkawrnbx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ukbgtyxf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2aubqehta.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2eojrlmwf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sbgkxevn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pugybiif.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hwslzlmx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vusyokkt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uwwkseot.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iwkufhbz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cvcxhxne.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiapphgy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bccfvfyw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2coyswqhb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zqcpgxrm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yuihqipd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jqdxgxeu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdmtpwpu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2txrlnnzg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zluvgppx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2osxzyyje.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ijkihokc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yokfseyd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2laxeulys.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2occchlaj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2acsapltw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lydqdkhx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2edtnzven.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2posunfdv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhyfobla.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nfhvtulj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bijjfvtj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fkttroge.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xbnurnuk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tjldhuem.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2naioombe.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mtcenkov.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lkzurqdk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jomhshje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkgzshad.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2obhgicfm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qlgusllw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ibfchsmf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yzovvarh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vycbbduy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaebymvm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hesmyjgy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2repxaueo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fykbezzi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zrgcsfyg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2plskfaor.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pymdestq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dfdeeuxr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2unnszonq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fduohwbx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fpjbqint.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ferykrti.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zearrvan.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kwkdifcs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2wkxblsiy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xilyryjn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aukbqqxy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pcxiungs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rohkblxx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rwwebglk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2msuzoyne.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dhrijkew.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mgsyzjmc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cigtiero.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2agamzquo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tgrggkft.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uactjtme.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqctcabt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvcqcgvn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2asqbwtyq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jlurslwl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2yzjkqxqm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hstsulkq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ayastrle.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fmrhtiuj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usfkpjrs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tbbunutq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2btdomkks.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hatctncn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zwyjzrjw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iapcqsnd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cdkoidta.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2owxcmefi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bhcmnqpl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yadeovod.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bakjstqg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uznwqete.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jydazjau.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2apkmwgbw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yznexmbm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2grhpwaqs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nmtupjqa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mnxliobv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mveewpaa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ftqtnzet.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tbilxdym.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehnqtrdi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ekysmxpi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tyxcohre.html


<!-- 参考信息 -->