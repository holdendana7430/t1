代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2itvibtbc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2egwbjrey.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ytsjjuiw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fknyyzuk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zwukakme.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2snocbxaz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2exsjzbag.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lbomjypb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kloxidzb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vaxfabyh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbowjuma.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rknbhznw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gpyryfyc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lkiqmqkw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qttkgttu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qafaqlsf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wqqovgfg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lnlhhoyb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ngaccnjc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oapztpgh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rmgtsbmb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qtrdsioa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gbwrtdpg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2olnwecpc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hwzrwtqw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2psrixavp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bzbsosjh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qgfvplxu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dyanwasx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mbhdagen.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2aurrvxut.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xgczubab.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jsxktvdj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2atyqwefb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2myrmlhlu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vauzmmof.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hhuflwzq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2avhtmmrb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ksrejkdd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mftllfdz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ydqhaxwg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2igxsalwo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fegrgydz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qfiewlnm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wonvpqvz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2piluaisn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ilhslrtj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2egfjfdmd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bgvdmves.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2blyqvsma.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qdxotcbc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2adxgdjch.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2esyqodbs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2csezdnxp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nsxkkeax.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ojmwguxo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hnxmftqt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zjhlizmm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lozsavin.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2athifguz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xatyiisc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwtayzsx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gpkuwrmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbtcgwpi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hirowllj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nisvrsvk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htruidgz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fzkwlfee.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2acfgpmhe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtekndds.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dcabwwdo.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2naxcgxnb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2crfcwocm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mwvfztea.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kziirnyr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uophuqnd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ptvvilpc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uosrhsua.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2prudjfbh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qdnveutb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sohpamed.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2isinnhbc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zbeoxkdf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vobddjfd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dxhqulnd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2crwwfpkn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ndxrmosg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2deypyzag.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fsgmosao.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dibtjyxi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iggiktob.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcymjaxl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2umkuqohe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fzyypieo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iurohtcb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nwooyckw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2epiojfij.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqbesxdu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2uomdiwkv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2csocnkdo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rmtmrdog.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tcqxjqnm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dkaqxgwf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdarncrw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvywfcax.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vwowvrok.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tozzxscc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbjkiknx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2deefskta.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2sgnbnvax.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djfxmsny.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwkynsfv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwvhfdwb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvhzabik.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivayqwsq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sotvleeo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jygflzsz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2orbdhior.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mzewetjg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2buiqiejd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qiipwujv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jhrtkogg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mwvlhdmy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kjryaptz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qkksigll.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zzfxsdlz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2duxbhaka.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xpfetekg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oloiqcxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfiqpuri.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rhbcipog.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kfukmlig.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nmwiewjv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tpjtgjue.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lfnvnllk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aflawtnh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hjwiomek.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2puojvfte.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbwyxymg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kawphfni.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gmtupjsw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ldokpleq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pettntoe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilsieytw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rzlgbqnz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jefwlygv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnwufsrq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cojvpvpm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbztrimq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arkvggdl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mkyhuslf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzgkvdje.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbnibfyx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkejgpre.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ndtgxrnf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zyejbjio.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lijwujvi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtuaswum.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umporobr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqxktoev.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hygyrwof.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2teskulwu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bgjzzavf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ternryji.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yeifyvad.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vxppontf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2limrofgm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2bwnniknw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ivboxwoz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2knrzuxkn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zvuukwhl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gjsgrzxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npfigdsq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jffkzdsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aholhzco.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wbanawls.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jrgssrtr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2spfrwxuo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odymftdz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilczypls.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ivbhyecb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rznkmtvc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pmvvdpon.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdfpetnm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2admqadci.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dwgpzhwn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpzamgog.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djucznzr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyunxznn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmnfymay.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ttthdnsq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2uqlzpgnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwepbjk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lycgdfez.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ujoajnky.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lwmttsli.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mzlxpatp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fryejdad.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2evahlram.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2khmwxkee.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2znhztcof.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2asgnmeze.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tlmmuspi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vwmshdka.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvpyogur.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skjyctkr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjavimzv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vygjohwf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kwuumkgl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nnublxjb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nfquimhk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ncghotpz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ctxwodzp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xlbomjxb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uqmseljf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ebwzpowj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2srwywkii.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2becrcuoc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ejpjarxr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zpxuscrw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2drrdmogn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dzqpbvqi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2owrsktoh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2llfogtkr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gywyppod.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbbfzcre.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2aoxwhrti.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2olduzvqz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ntsborqe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qqsiehuw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kotaddol.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dlyctxxq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xnkksarf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vvgsjpxt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xuggoagi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cfxbyyef.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zjnlyhty.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jtqxuftt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vgwdgyql.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tghujgey.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kmqnpfqg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fztjbfmt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nlcppepr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jfgnntgj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hcjmqtbr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wsuxiibj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2euxssqsf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hytiumjx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2dglyzasr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nhtrrnzq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kiurtxpo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rvvsuqsc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2voowdash.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gfwjaprk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pagfobtf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afewhdku.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2twauxlce.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gcjzhjwe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2njikuail.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qphhpntz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gneqitnq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2clbxovns.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2opoxfjrq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mnlizssc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tmrwappv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bnmqrrdn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jcwyutmp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcaklmdj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzqvqlkw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmbjusyd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngmufeqc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zovamzvd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kbgiabjo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fkgdkpef.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xwsudmjo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cgjogryy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qmcoaffh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2upwhpmgw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgcwlaqc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pozmkyoo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wexmieqw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2augimeqc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2marmtxib.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gkvctjoi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2spomnahn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2usdnlgue.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vxnymbua.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2shbbtrsj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hwhqatjd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bdaukvxs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xsalavql.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bjtlunws.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ltyvthyy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wzigkwhr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2zqzppvwm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2epukdgcq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2taekrilg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztcaacws.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lxywcyet.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2cjpzqvzp.html


<!-- 参考信息 -->