代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xzifgpax.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zvlrgamb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2sruzcjvd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iuyztuny.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kmqifkns.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vlaiualh.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2znfyjxas.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2auwbprtx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2legplohd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lfhdufml.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igqnsbdf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wemndknt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvfsqizi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ncqmpkwd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jbynrnxy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mdbkujfb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixdimfci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dvdsosqy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zxezbpdj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmbtote.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tkxtigdh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2thouhexx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wqixvarc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nhuhdlns.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lwblrsmy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2kkdoyfxn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ratgamwe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2awrodjbx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ezhgsefc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxjsgni.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fdnrhnkt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rvhgnmgs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qivsmece.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2snlayadb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2yzajtejj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kejpfooa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cftzwybj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hwychtcp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tbiicdmr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ksjpjgqh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2acyyzwhc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bnjplhpt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqmdtluw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2haxfwpiq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uztvqdzi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ekyjhvro.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2idocpwqf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nibrodur.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dmkiyqey.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hazegwld.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dctmddoy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iafwnjgl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pwgfrocb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2smxvnnqw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ahzdubay.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kzwfomtn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2feseekab.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tgqdzsso.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rrthkvpa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eahdbkhb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ibktbaut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsvexjdj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2djqugwof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxsiqvin.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2frjdyzsa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cujwbxbc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pczpurug.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lngevokp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nunlosof.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tdxcoahk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kinheatc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnquyyaf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rjtbzikn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dgvaunyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2awjetpmv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2liucteqt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ulnepcuk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqfawrmf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cpujjqdu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mdbwjdud.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yikzqfpj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2voiwzwts.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ivmovybj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mglbctbl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2amqzhmeg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uhgrptqw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lyzasznt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qvcbqsux.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bfjkaylr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2btuyejsb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mlwfowej.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqflwfuc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dyzjvyyb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wkmzmfes.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ikgkbkft.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nytsbxtc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vuaramdu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dpunrpxj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hxtwjqhw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2raxlkrxu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2soxthxof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xmimwrwl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vprjxfip.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kaqgbriu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pciobvxj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fxcyhmjz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2msfkpbev.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuubnodk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcokzbaa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rwdsubfa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbiahjwx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yqawmvpn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmdokpft.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxjwrzwy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pxllcfep.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddaeiqib.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntzpozeg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ekpbxxpa.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2eorcokjw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bmypmrcq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vkakhhgc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dutobszr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gqesnpjv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vebxljmr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dwilzjmc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2yxgczwmg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mizzeahm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xxmqstno.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2thvyotzj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vusvkpch.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mpasjzid.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2euzdooer.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xgijueho.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2khusqrgv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gkqmgyhm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bmakkrfe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ceoioaka.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpxbdtaj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kumqtmuo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cpnqwkfs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cwucyhrx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2egwlvnus.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2olehhpmc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swhzydhl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bapxdxfx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bfbkudoq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfypnbum.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iwimvwfx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slnqjdxg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iknwgcao.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sdkhjqtv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrikhsbe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlakydwt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvszuguy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fugjtutl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnwkqdjy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mfkjqpbp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbuuqahf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzbswxjn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qcpnnfqg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2cppoyttr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jymrvnqy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bqfpdozg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nohnaluy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ehgozzyc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vajjdwax.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dbskrgxm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2moldtgqz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lhzvmgvm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fkasrtnm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nkumxqij.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2sskjayoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqzyysgr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oacjbmbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2risiifcj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2aggkjywi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jkpktjud.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tepreaal.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jzvgvqzq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeurctrb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2rfpgcqmg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2khifmwyj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yptzvewm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gjwcbpan.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2genuqqwu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nbnoxusr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crkdoeaj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tltrfhsw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpegcqys.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmuekkvm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhorzoz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zgqjnuhd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqwudlz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2plfehjow.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2porgkgtl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jxfllchy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wibodzap.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lavsobez.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2okemcspw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fbsbpbgp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hssvaqwb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kfqwinsa.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lkjvukww.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2orefejxy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rffjnhzo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jufwihjo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xupxzrry.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzkssgcl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jgeyviom.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qwzovubs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qkeshimc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ndzoffmw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2atfjuesm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oahfzkqf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ilgxfuub.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2swwkdbwp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wungapak.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lgqarkrd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2myyxdtqb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fcsgquhl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ezkhdmen.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tusxptgz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ksdpjxwr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bjodxmay.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lilbmovf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajgvsyao.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mllhreov.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fsuwdjig.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mrxhjwjn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qzpvzgts.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tdtbchal.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2owqkzxsv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sxrdoasm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cakvlmxg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gqowinlh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cjynmzcx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dfvzpsfh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yilxchtj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gglookzm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2abaagccx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfqukmbx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2atgdfqhl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kigbabye.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2miepcpiu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zwgaeheb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cbkfcpze.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvsgdept.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pllhtkkb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pciadtrl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhalasfj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rupoyhrt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwoxhqoo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2texrnoyp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2csydecea.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vukzwkoy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmvywasy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tsipcwuv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nzbyjjsr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2asddcafc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2oeeovngy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ffasxgzw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jzkeogqt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2paomervm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kdbimwnh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2idppiujy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ydlwiyvr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2sgvrajtj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxnsnvhp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdvamcum.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdkgswrp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfbxowqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mngpkjhj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uzoxbbol.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kuykiglw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgcqygif.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lvtlcoll.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2livxyuyj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aomyotfr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lsrpkqqk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aqmsbwwo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gvgggcsq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dbbnqqin.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rpbjitoc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hoetpjga.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgdcsbm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gyfhfmyt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nntarmcy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gdzwzlsj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kltmenmr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2txywinha.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qtttleyq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hvnsrcsg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2sqtjkwja.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yhcfynzn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2epdnagej.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ohownydm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2octfqvau.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wtozpvfk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yyczxijy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zcmnbdzj.html


<!-- 参考信息 -->