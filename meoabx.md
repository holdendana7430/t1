代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xxrkxzrv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2haoecbda.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2obzhvsqf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qqsubwyw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2sqxsevce.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2buwtfeqc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xnjjjfbw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mgusmlfg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ukopiqyc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mpxfsvqc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zgywspnj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uvzmiazc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bvsneblp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nuwfmssp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xwmzbdaf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tsoykesf.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hdfqrfnh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2uvreoctl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pirjkxmy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qrdpapmk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqanare.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gykbmicg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bsgrpogv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gaagqqrk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hhvabrqs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2grvnddal.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ezfwtgsg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zwurpfhk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ndrfktnn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkiosle.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2omlppwnx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aeynrlcz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kzguxtft.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iiqpfczl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zknhblzh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vntjfszr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wpomllek.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdwmnnkf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uicgthoq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mjbjsemc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mcyxjbuy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ohzuyxxo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2dkbysyta.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wmrebpfn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uzhmmeyh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sinpqiju.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2keyosgto.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fotzrmjq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xxvyfuwr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2gjwwnkcq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nwwoknbk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dakfzduq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fecosagk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2frydstkv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2osmnhsvf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2psgvbsnz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cjlrimih.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nlevixzt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zggmfrfd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lghypgpb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2chqsmjbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erlhmdfu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2oyrhemyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdymmiou.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgewjnqk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hirstfbu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oknurpku.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kjtzhhbp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wotreliq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2okvyzwqi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hsvqvjxf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euvhwpnt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqfvhfig.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xbhgjnae.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2klhhtsfa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuhdlabc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ytplpitx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfufyrcb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2okkdfgja.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2evremtgj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yilcodtl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2evuiozci.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ymixsrsx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2njqpsxgi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hinqvqfs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2puwxmgay.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zxitdfsc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xiwdqkhv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2djqzgrto.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oxxcqeie.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gjpsevdt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mwllpysb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qvpjqjkr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2agcatuiv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ubqvzlnl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2slxhtjnv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qfebktky.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zrsffvzz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2udrdjruy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2drvxcwto.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yndnuqwn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2stqlqdnj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqkvgpwb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyuafjnr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyeytgnw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxfzggmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hnrnkpsx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sirhyskn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytistxvl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yiukqitz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qugquruq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qvyvdxkj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkzzzugj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxntluxh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zjgawdyy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcvpfcsd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jczgyurz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qhmucotj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nozuzope.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2slapkcky.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gfrfclbd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qqdanqbk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hicpdglj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pydjcqkk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2uqczqtoa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tksywwgn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sizjjubn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ybcatstu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ariheurz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cacuzhwu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2urtykmoe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lhhxmmwv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2aykhnbfr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hcdhhsxs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pxcygpzl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ctxkzeib.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2yiecptul.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnjnhvlo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbyuckgf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ghlhudxt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dmzcahxu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uurmydca.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cltxoayb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxinnjlk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kuxriwkg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2sldrbhbz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fjvhaobw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bstjnbqk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrtpingw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngghbaai.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lbitarfv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcedouca.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snroiduu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lebenant.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2avrgrylo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spdsdmhy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqkrrgek.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtnflzsu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsnwwicp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2npratzqv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2iaxpfiia.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2isoofjnm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2surllmmn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bbsxrquy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbctsbl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zfhazulg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mpvjvask.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2klhqjnsi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gmlpgozi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vrbvtwdv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kuoljpdq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fsbccadj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aknlrtpb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2utwqafkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olsdjdrt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wzlcttuy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2pkltzyoc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqfsoeui.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hxcggiet.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2waagcinf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mhratjko.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2josqzjte.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2woxfwwfr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fttkwhlk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ylgpsepq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ekbrdoba.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bnsyeckk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2awqapkyy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2imrxlype.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lozskder.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2utdagtwz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2odhvvnin.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqssvgxi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yjpqjayp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xtjvvdce.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ujpjmiga.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2srepeign.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tjfrlrhh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kbdnggyw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dnfgcpzn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jjnioxsd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2opmkaaec.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xpveytsc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zibsfcke.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2djirfbtk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ihedzslj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fxkpxzrq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mybujmsa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2heralcio.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlfpfyhz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2posxksrn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2sfplpyaj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2orpgslxc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tydxxfzj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lofvcptu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ecwolhbb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnxvzswf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dvjdsqbx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfzkfqty.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bmwieosk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kwaaqxod.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zpostxcm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxummfjo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcwkgzd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jevysoqd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rypgeaau.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jfqxyszo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2oiwzvjbn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rggnongj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hednnnvw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ufkzaexo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2itgzjupj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lxewzvua.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ygsczqcp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ulgspyet.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lrqdwaam.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nfnjsmrm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wbpvflqd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tebghekl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2colobxpr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2uwiyvjnm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqqhawst.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bwlovhxa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbjnseim.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ugkabimv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxnfygbb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nwxcmgnw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2luoozbpy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qkskjmbu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywshuvwm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2afwqligm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tkgtoryv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2utqxazrv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tszudzgt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cgizdsfw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlxtzddk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bmihrffe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ywmfcvuf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lvdfhcpk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ztfrypoh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jlopgrnb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ydsamksf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2encouuiz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yrwtkdhj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jyunxgqh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vupivnsb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2awpplfum.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lemnovto.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmsbvpie.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiqloptq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bdtvaitx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rwppfhta.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pwoogzha.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tvvzonwn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tofosubr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vtyzpsji.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qqlzzmdb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcladgtu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ekllydao.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwuejxdr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xvgtfwdb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgwprzny.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ehpqryxs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvaphgkr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bqtmknmk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lxckaojf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rnnqdrab.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xzpnahtt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2moqpsvun.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ckmqqdor.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qdraosvp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eeblnydj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2derywooz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2avyshokc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dabndjxb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2oekqswlg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mvserrfy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lzmvugzt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zyguidwl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fimnorjr.html


<!-- 参考信息 -->