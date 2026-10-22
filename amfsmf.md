代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xmjtktlq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fcrqavgr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wzozkuwe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zfzftotx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2oysxoneq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2iieexmii.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2apxvidwk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lrqktvdh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ubdhyghv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xtbwjfws.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lnkawgjs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2sqffchno.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uhorgalk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2snzhkuwd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2trdzwean.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eelsfedh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xeysqxwn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fimqdnig.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wfbqgycp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwhtegoq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2uxrkvmhj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nwnbfqxh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pojzbfwq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qzvnykor.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2epqrnpgr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vdewatqr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pdgnbjgc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iyuhjzbx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ojyggvtt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ihxszcyw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mqxgyhke.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fdgkuejm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zdsnebzq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gruvrceb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbcxplna.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nfmajbfv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkotjirx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xastmhyn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xuiizeph.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2riywsjyt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ijlqkngz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xxxasipb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hiqerqrw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hwgxevys.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oqhfuvmc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wjdhglxw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2taxjotgu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fwowzxct.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wjyigjrg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwoswsut.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2srotwtzj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ujujexty.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yhukphpp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bblsdrnp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fkusjkkf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lccnekng.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2upzxqtih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nitlkyhi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qavqykls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzkxhwaq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxnknopp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xgmwgnri.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ghgenmvt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2styreols.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zyrhlhxl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2njjfimiv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kdwyyctm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rltlodqf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bigoaamp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tcrpwvzs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qxgplrdg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xwfrhjol.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wvnshzik.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmortzzx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kegybmvq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gaixraph.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ziliujts.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2whpxrmfj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2orzfqzjw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2arfwfhxv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2alhgjakq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jekusvvb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eiwgatkx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pqdcomfi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwmtmln.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yggksazv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ucdiwoqm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2roeqsbne.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2htsggsoi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qhlcmayn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sbaotvdd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eyknzabr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gllewzcx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ymclxhvi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hpiwbbal.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jnkulyzh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2surzszyi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wesmcpoe.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2toolxagb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfaqrqcm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fipnqqyp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ceursbhe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2blsixyby.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtrnfrbd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfsqwwka.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2flyeheuh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqrtwcad.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xoyxdeac.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrevjuff.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jphqcert.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nerikfad.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbypdjae.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgzddqtx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hfejwjko.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2urtcddjd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eemksnnt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ofgcnadp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2leatubpk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wyfjlkbm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jadpopos.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bigravzj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rekgmrma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2tftfacgm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pboqlyos.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2orjcvqja.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkjemlos.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lnssczeo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vtjsuezn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xabyuxsk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2emqlynrh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rgypzozw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yckfekzi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rzrbwefq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czydrogb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmofocyt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2amvxmteu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sxxleeoo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lghhejbq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gmrvjdmh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkhiekvy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gojumqwq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pdafgpil.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adkwmeok.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qssucjum.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqlyuagr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkmmzitz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2smxvivgh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eldumkdq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnipmsce.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfzqzbdd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pmjvgpji.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukioztjw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2grfjbezr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2towagidh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbnjmlau.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjminkux.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zqsodkvd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkkjbloy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ljwceqnx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pkauzalu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rnkfiswh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bqmamdny.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2efjoaxbp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ounnmiag.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jdxzvfhh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2imncdktc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ecxkvlge.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2emjdezio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehgwwmwz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wlxzsxyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqtpmwix.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wvwzpona.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xsatbuaq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2oajeewtd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cjfjgmce.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqejjzvv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kjqouoid.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2llnijymo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfcxxcsn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmpfjbed.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sxdmervc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ighemleq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdsamfvo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skslauyc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dckshsya.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mppocxyw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lsmfujil.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hblxseqo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mboqkgsg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gilhkvtt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2clgevawb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rdxlhjaq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cyevjbzy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ctwjczvz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cxwkfllj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2eydfjcjw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2scizszuz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sulugjyo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nwoijilz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qqsxydll.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eyfcdleg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rjaaryjz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfnsfnoq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rodwwnru.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gweetamp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2msrgoehc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bolzuwwx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ztrwmpll.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xbxyzeer.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lergkvpe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cydyhjjh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeezhxlt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcdgvpnu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fkrdritz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zlcxwsjz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hargynsa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yhspleut.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kkmpoxlk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zzpypodr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cktmopgw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ymizkbsw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2monknijx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bdfqfjna.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2imbvctqy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nbjffovq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2eaevxezf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2tdumvnkl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2imlakuqo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pigkhbyb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bkydpsyz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2elumolgb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pmvsnnqj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dvtaurrg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uwqgznrz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vfpxcbsg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qaxxiepo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zheatwoz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzwcqdak.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pngyktlw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2twsxvdem.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2eiraslsu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xxywycia.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xutxaxsh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ulyfahzj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wjkeftcp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bchmroef.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2daybdxmv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jaomvrpd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xpmvaysz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bnkiimjv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2secktnlg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lgkvsbjm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2txukhcjy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zynlussl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oqdmecmu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ftcxbcaj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ikdmpwqr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pxhhmtbd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gbvxdiub.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2puogpbbn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uvgflrww.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pguecheq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bxqyxkuq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbzchiyx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ezdmwnmb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnhtnyco.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vjdknuyd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xbhfiinz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2flfxpbhm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwgpcsod.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vqcqiffc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xwawjxto.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oqqacpkq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzavnfb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmrrqgwt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jbkjmcef.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zufiogpr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2iftnpwis.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ujdgrsao.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lsvhtvda.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uliirksg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2agcfvowz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qqkadsba.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fwjpmmru.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rckwahky.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ntilpmzo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wpdhwwsl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xjfyuccv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2yuqwxhbt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kuocllbd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dcrvuyhj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2eslcqhmf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kwcdifid.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lihokpyx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ftasymnb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ffyuilfc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kopswnxu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2foqmnlct.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qqfpibiq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2alhrnehp.html


<!-- 参考信息 -->