代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kmsdykhj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jynijyjn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrdwhjl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgufxisa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2aagafytj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vkhbyxzh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xejsowti.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hqoprlnc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zwhfojhh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qbxqfygb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vvkcyjsb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhiiuup.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2prrcdrze.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yakyrqlt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tcomwbok.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ovmupcbu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dkvagihx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2taeqjtot.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hyhowugx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mmycjmnb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cyjyxyqo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqskecn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qjrwihwi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rwagxgwh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kixuffsi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zciuxngs.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2uonuhogs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2damteivg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ockawfoe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktingihc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkjhhgaf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbciiunk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lttmnsvo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zqugwsxf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fysbtaex.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tagfozve.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2sikqocjd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2noriwbjx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2epoqexch.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tckxpaal.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qzcvbpwe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lnrxqwyl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2suclusbm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2botcsnag.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hfhjvugt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxhxvzuf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2znwxqqvg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqguvicb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dvjnopan.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ciutwutm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wvxebdpu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pysvkxmd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cuhfowjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdrewtwf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qrpdysvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvfpckds.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2duselach.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mmogufvt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lssmhhke.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fjolgwdi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2exlgmkjf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zwtjregd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2budbzozh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxtochuq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cjpahsnz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpjutmpk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kgypsacq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvydnuca.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vaukhffh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mtroalzw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nuhdycyi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2llnivxdk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yrswuoma.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jvepcgpl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kvqcphog.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hiryijrn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wekbujxx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uudlbbyj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xlgrtdmn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qjdwdpnb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ixkgvfxi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oqagwric.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mynnowsw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lbdszqzh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2scpcmaeo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yfdozcnt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eprzytfo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ddqekufh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rmanxciv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2thijybow.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rjgvncij.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hdwcszxx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zaiblzxy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2inlppzpb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2niebnucl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejtgyuzr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwhtcwpj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2miaurmnc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2votbzure.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmwpumzb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqxxrrge.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kzgagflv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvlxezjd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzthlqvu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mltycchg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtscofjr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qighcuvw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpheerxp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwmhianh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhwvajbx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ppwqkdei.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gujfibwu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gbxqguei.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pbzziabd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tsojszla.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rkdvjthb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eqhjvwnm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ozvpkwpx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2meyfxqmn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2czesxdwv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxkmxjk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dflfisly.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fgfcruyf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tnoniksk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kcqeqyaj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nqnupdom.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hllqhwvx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2swidifdo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nmgbxczo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbkinydv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zlygqdat.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2brrkdwao.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tfrpsadz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fcspurqn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2svnsimjh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvwvocil.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hyseruhz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2osazhxxq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2auzxlprl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vkztirbd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ekrswjaz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkzdjbbn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ondcvngv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdkjyhvc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oeslthba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrduprow.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mligqqfe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtuofasq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tupxecyr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgtxmusu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovtqlzby.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrextqz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2utxrxwrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jxshotkx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2athmaaqm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2upgxoxjt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yxdkywzv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2thhforod.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uxbpmtea.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kcsdskeq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2urudfyvv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ukbydxzx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yomwunyo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rwamsrta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdbvtfyb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gdvmtziu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvkvklxa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2giylkufu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2amnnojqy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2efnphtwr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmkmxxup.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2milvzmxu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbrixkkf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2aszisgix.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2slcdvzou.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2avojxphd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylobkcaj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qxggchqx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpzxlgaz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxwqemay.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gwfxynuj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qswjjufe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fqlfamsy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qdhnovkk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfhxbhzs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2oraqcduk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oezjjdfj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wlbnibxk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pijubfec.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tfhigvey.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kqjuoqen.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mtxekqxm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rmohsyvy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wckhyjgd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tzuykokh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hmozzvzq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mpcplneo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzgqamwj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xnxhgmpq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wbpusbgb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wtmcjuig.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ybztwome.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ecdssgmc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2spocrhnp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wdcjjjtb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2orynbxvj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlxrjnpz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlwyqowm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfooavuf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rioyhtpn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nrigxcvr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wwlgoxkz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vjijjwta.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qhepleug.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lazcthbp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yeqrcpqg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wnwonany.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jvgbgbhb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2noutlyas.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2cadbbotf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dvukqauu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mrpqeyxn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2aghdroze.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gkmsyqza.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akkvyklt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2icafrbsu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uqrbqwkw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jhtqxcoz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ylqadbqq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ndeijjbm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2aaqaxabm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cbcgfhdw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxmzuzkv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bumpvcvb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdyihayk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pubcqbuj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tgrbrora.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2szswxfex.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhjhvukd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bbyxgejl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ilaaaria.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpgmbord.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oiidbiai.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wnkrxhwq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhbvrzsd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cxwaasze.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tavsxckb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpompijf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2icfzzxqh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2esnilpso.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2toampcba.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kqgaytjm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ljhctvxm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dzonmgix.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rknfpqlg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mrcxtpvb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rxwrkewt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zdtgzlef.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ceqtcfbi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mibnssmn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nykkxylf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgwovbnc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tpmzxkof.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tizvyfop.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2micsdaun.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssbzkfoa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hgsnhvof.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uyqdanag.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frawhddq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnipnkeg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcdldezx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpqdhji.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mmcqguke.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vgwunuiz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kwthpizf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qdjwlrkm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ykkukufg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fjvlvdgs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hdejbjtv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gtmiwyos.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hijzkpou.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2oyaxaqvu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhczbfv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uyrwuwlv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vaqxtsjy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lgoryzrp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jjwlrrgt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2guvsdkzc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2msdrcnir.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epkiniuo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2onvewbfi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vitpqqst.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jvcqctop.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ntclflza.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2owgjrvep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2opvataup.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pvlvzixe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2duazhtyn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tbxbqupo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yizlfilm.html


<!-- 参考信息 -->