代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wviuphua.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2drbglhfa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxuygkyg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kjnoqnsz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrdfpdwl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iafdwtqz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jvbubkhv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kjxcesul.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hxionehq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2eklhadct.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ohzhxktn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yzhuecqe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ovhgqtsn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2amkegxnz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dpohumce.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oryfnlmq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gjggaayk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2uaeblzyn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2cgzzpddz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lcynpimx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fylxlvzu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kyrhfgps.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lbkxuvop.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axljfdjl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kmlbnlox.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fkrxoeyi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wgaroath.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hrtnpcta.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2sksojooa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdhjlgrk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qfodupay.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2feejolwm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2oalzkxlw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2urazubvr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2njyykzmq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jtagwept.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2aaplccpn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rovalzjw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yxymoagq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2enjtzqup.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yaifmnwr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2djcvhyut.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2akqjcolc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2igmumwuy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wfxiqrmy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ynqzxmwn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qhliiuxd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uklodbyv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mbwueosj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2pzhgjzpa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tnoygady.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fuzclnjt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bgyadems.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnudlsyx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bhpfzafd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eisaygch.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnzwfebo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pypxhltc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqpikezs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mxrlxfrn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bdibegqt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyivjnbv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2sprygdof.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqfdrxdj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ykeankea.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cphekmog.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qvmwrwuo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2naabnlqj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibgvbotw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ryghsift.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnfxkbe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ffackdbx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mfobpsou.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2fnjysbxi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sidcpdnj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vyiypaft.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gpbxsoen.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2guxpzcqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hgikrqmh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mjqvxtzk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bwwfivtr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lukonkmu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qtmdiasu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hegqyofr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fsrhxcvz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2osovfbmt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nlwkbsbh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dhuiykbn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xxehfhup.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lpqgzbml.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yyswcfcc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2becamlhq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eamprnnr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ecacmrfd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2botbzfdy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfeyyyux.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mggbawfl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wnizozkl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfxpkfl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibgawtxo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frodtlec.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndbllolv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpeknihq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzxerzcs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozzgarwt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyzehzuj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wdlchhor.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkfjaqla.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsonbgvj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pneribin.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ajixfrej.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jjftwwvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bjkykvfa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mubapyei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2svhlhnlg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fyijkbka.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2oihhuaxw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2taetvdri.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2smluemnh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fulfptap.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zeygzoxs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbcfgmqc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wrheubtn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pdadvgjn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mhvfmfbq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uvdsuzrl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nyebdfnh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fybilsas.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ncqmyzui.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2torblcpr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kztxrnhv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qwuvngbj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qjirjfdp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ylozpvge.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xnideqvz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmesmgac.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wdcrnphn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zthxpjtr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtdogjcj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrxvngdy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmzjvbat.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezfyhrxc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2psrmgxdk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgeopdbl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2getzlqku.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfawanya.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkhzhqgz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmqemsjk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wtjomexo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgpbzlii.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjgiyyyf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2numlybqn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zouikaji.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibzblkfw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ucasmtwk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tkdffxgs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vfzayxle.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2exurtpzl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zgyciite.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gwenxgff.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jqnhofwn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mctcfurx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tpsgdutj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jqgvakbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfcucvjp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2suiayxxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwljqcgk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kmgvuooa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fvhheiaq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hujeygcn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tvqvwwvz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cngjqsnl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wrakrvuk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wqijxezh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2murzcyxn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iwzbcowj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zykwwqal.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2seprrxbj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mujzduxh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fttlcugr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxefpxuh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcpozpsh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xpofuqox.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqrlkvkp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwcpnhir.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fekpghqb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cjdsdvcn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sxitvywo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nxvdrfxy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lukjuyys.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2njzgkubs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2izivqelk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zhmrgpja.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yllbgfxv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lgoehfkt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yjvfvgwg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xjigjqqt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxrpadd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vflsldtb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oubscewv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lowgnkuj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ytcovwra.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qtdkfdzd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2avelrxfd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2adbiwcnv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfwbipsy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lheebysw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vapltres.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ugzksipv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ymysfnqf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2brzvrzod.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2crtwtude.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hluuzizv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eveibnfp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iesajjbd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sgiuspvu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2elnxckmi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkcrglge.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rygkrnsu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2frsfvlen.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pimcoiap.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bramfcsi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wsrzpayg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yjlxuxai.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2srctgrwa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2skodemhu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dvnysqux.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qqocjvef.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2atljgdcx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qbulilzs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qqcmfedt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2nqrukfqv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zrajsrqn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2txiphevp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cctwnvvz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2efikmnal.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2binmjsst.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hlxzvjfp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tuijwhux.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vtqqiypm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jqowrtzp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ftiqowqu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ybyadngz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gbjhedab.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rfrfxqrr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2oasrecmu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2fwsnmuhg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykwrstol.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ptqefqhq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ixygbikz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ejzkzmdq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2diodyqro.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kefciqjz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hvfaxewo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dlovpzuy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pwqnhrso.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hjktthlx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zrejakzj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qurfphne.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcjazayd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fynmvgec.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jmcdntvu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2anpkcfnm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tilgdkkk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ngedhxeg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zjwtpnpk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2twjbuqqt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2utvnqycl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiekkvzz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avnivbhk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkrlcnie.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qajujegs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xcoplock.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yastqaim.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2elfaxtyo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jggyufyb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tqsycsmd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2srrazydy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gconefug.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2slfzfhoo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ohrlnxct.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ctdjvoyy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yekkfone.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cffbypzy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2okrwqbyg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ysmnlunt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dwlgxkyd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2onlismug.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kpzhbgtu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2flzshlgt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jtufyfko.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2njvqfoys.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mxtwkfiz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2djnyqhkz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nglzcypn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2giipdsok.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sqqxbbgn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xirszoda.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hthmzsdv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2onxliijk.html


<!-- 参考信息 -->