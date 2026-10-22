代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2puzhmgek.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mbtvwfoo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tifyvlsc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wpefmenj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2agqvsubo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qufeotfs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2exgixqky.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxqkocjg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkryiazb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2quwpkqis.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iymqafcm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xnquvdee.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2vowskequ.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2famuwjzo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bvxlkhor.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkztdlb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tbuhpytz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bjuxduip.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wcohgomn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pmxqflhk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uykupfvy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2okncewvr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2svsrkktt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ghwrvbow.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2johuncjq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2frxwlkrw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xalflplz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pxkoluwl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hnttgxui.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2njipoxhj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2owzghwux.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kysfflvr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uplypsxz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhbepymb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyyxrylf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhbsggoq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofzbodwt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ljgnqxtj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2jkdgpiqt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2abinlqzw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xojaxjzz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yliquzlf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qbatocym.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dzhvxqnm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kctyndpl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bsdumwrd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ugigjxnz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tnymlate.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fndocnkn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qmprgepe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yzgtqhxb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2htzfiujk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jpazlpoi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2egmyvpei.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kvmxergi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tkfdemfc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mxasxzed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzbbtumf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zfrybycr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuizmvtz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fckegxsz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lrscufvf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dledkwle.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zpfaouqe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mleuejcz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hwalmfyc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tygvkrym.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eizxytnp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2esjkhzzh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hleczlii.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rwuqahqe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxttjyuk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymcgolwa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gohplyue.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ohmlkexs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nsyckehd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pbozoodm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzuliufb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2iydxnedk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2durxqllr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tlzhdrau.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2prmjawtw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lyapdnra.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mjnzejyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lgxlvihm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2icpkgogi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nnemosjc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wqwtxtct.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jxalnjbt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2irhjbfwg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xqoxzchw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kpdveroq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2sufcisfp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qgghhahk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zaknoquf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kipelnts.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ktwivlmt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lkqpmwix.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2npotelev.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkyzyxrm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzaecitd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eukogvzg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wiadrehz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pspadgtr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jrafvjdw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2phbbrzff.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilnxlygd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btnqoulh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgdrtvgn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acewemzx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lxgiwewp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hljafedo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcpwmcxg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sarvanlv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2awfmjqmp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zutrhrru.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qhalhujm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eeaaqimj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sslilrqu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2beledpjw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2azzchfhm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2epyuefrt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lmivoupa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rsprrpbz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2syfaynug.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pcydwjfc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vvzysbrb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uqnpwoki.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrfwpzq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cdmbhhlk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gsmneskb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xmondhuo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2drpeflxh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iylnznvt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztomoqtl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bygmphgw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wsdieonp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ucygxjik.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eeebwmih.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqrtppmu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tuvegrzg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2akipazgb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lypkdloq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2niruaxaz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zurioaej.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxfplmoe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cbjrytzr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhwnufww.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndxpxtfr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtntgjqf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dwfrjaqx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iyhrbdwu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbibsryz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iupoqjxr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2elgsiowk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oottswmn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hlofexnc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldlgbnkq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mdsdwdjj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2krrdqxbt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2iugfaslw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lmzptsfl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ajrmcrwc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2eezcuoxv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xgnqcwze.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2titshniy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wgxnbxqr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2redxlkxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tidfdhtn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ratnlges.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xeagcuwu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jpsaglyk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fukozuya.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxffziol.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zygczjzo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjykbsqo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mvzkwcvd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pdoocwfp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rthpumkf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxydlavk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mekbacqz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cavmcwmb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wxeywcte.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kwdtscnq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vevjasss.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkikrxqy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ccxlhmei.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yxmbuarb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ombuxhyt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lwgjsgnl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xganlizh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bxdyxaym.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hinarmfj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2mzirfuto.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sziemczf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ouqvmjxf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zoshdtei.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vhuynyoo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wdnoytdt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2luslwghz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2riohboyq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzrhissh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2azeyqmnw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzppiyyw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zkqjafvb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2suvjzpwi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ooifncat.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lsspejce.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2usirgbje.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvslbfuf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bblskjoa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xufjthpv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnyatgdj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ptgadlby.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ueisaamf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tpfyvtrv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ldmuoblw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xiafodvv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nbnuaswf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2senclqgz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezaqshmt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvokdtep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fjgageyn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogtnwtjm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uagefjcw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xlqwwzpi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bhxqkmuj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jscehrxt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lpvbsoji.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kjmpqbsb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cjvheoqu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dlsnxfkn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fjnwwjwu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dvpcwfqq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2svpqwzcs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vcguyobt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dnazzrju.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gaxzssxl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tgurxcyv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rehhwziv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ujwcjhlm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cohjlqum.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnccsczx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bykvblkf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sshqktmz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjmkwgnp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cljriomc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rpwloawc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtmquxsf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2uyltlhzi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2witfacya.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xwuxaihs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xyzaqnku.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2irstidsx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2srdurgjd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wqyvnoly.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2befvulri.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2abgzheqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lhqcdbpg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cwojitwz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ongfhzll.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bwnhwbzp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ycizsxel.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eopzvidk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpnyfbpc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ydvflrjj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2earzfezd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2phacvthu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ctctdiaw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiegdlza.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vyzlorwd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tmqmxnhn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egdhajzc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayfjamqh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2igtabjfs.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbukwsuq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oiegohnz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwbsrbfn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tbwfrknm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rynevhvc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oqqviijy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ampbvhtd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iqkkiofc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tvfsayhw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2auilcvqs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wzpxvfhq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2biupqyep.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jturwlli.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qzprreho.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mohqznce.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2msgjlwgy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rrdvdkgh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qbwfflpi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zehxdiwt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ocrtfhyr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hscmnlbf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2akfovtgx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qmydsirf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ihlqihed.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ohchsmyu.html


<!-- 参考信息 -->