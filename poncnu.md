代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwjuhuat.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bevsoizq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lqnufqws.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gnfsoedo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mwcmcdnc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2eiuewxqu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tywmhodn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gllpzjss.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2izuhmpxg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gfexeynf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ajitopyq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2edwdorap.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yfdhxpbi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2islfvztg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ibhzgmku.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjpbjllq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pcewmetx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ilokkoox.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2javnzfmx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bssjnhih.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rldthzys.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pixukvju.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mojpqlov.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bnhqkpvc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bifmjqgg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qfrjojba.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlfcgzhy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyhubghg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xwatagtd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2arzegviw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2jiedyway.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gbsestgv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xyyktsgg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qasxyrlb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2irbdhvjp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ztwodmtj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uenvfrok.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2btkfiucp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2buztjoaw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ikzakcnn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yohdnogi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngaksmss.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vezgmpue.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jipfieir.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bregijcn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2spvvnbyy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2khhnovgg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gqldhgld.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wbehhuxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdpoeskx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rwwmeyds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtsqbswj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cgngbjln.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2imcnqmhw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yxixzpbz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2anlnwlqu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pxjantaj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2veocrctt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pchxwdnl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfsywila.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jpvqxkfr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2swiogmoh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tnnppirk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfmoxdkh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cwcpyhrv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xeenmeri.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ftwmqlwj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fbphrgsc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2umcqofqu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjqdeuqm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xyoagsms.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oiuecmfe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jngzfxnb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jlnbsbtr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2acwjzhfd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2anwxhfyz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2aqacfjew.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2sfevmhcf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2embccxni.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhgwwyah.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rumgkyai.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dnjuguak.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vsvudcnj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kxrnbgge.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lfcvdotd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2immijcvh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wmixcoxr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fktugfcr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2scpjsurx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rjxmhddi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dejleblj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngtioutc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxmivevp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyleggxl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2irtrghbl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uphhbllc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksedwajr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2shbfkvyw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckupljry.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kysddylq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poddhnad.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aotaytqb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bgibmywl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukasuqmc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkikooqr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tmztkkqr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wwojtxfh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vzkupefg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dcntqwyy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bqupjjbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2spuhjckb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2yvjwncej.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2isfrmouu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qrbuaicu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xtvqlepb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uwcsonrh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fufombdy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ensunsxh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fbllpxiw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uwzcfdzn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pzznugxq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lenwojqy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kvxulfig.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ndymiplc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xijrfwpb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdscvlnv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gstsexug.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2krgpadcu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2typztolh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ufmvtxwh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2csrbpngm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfdpmkga.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2spdacide.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lvcribff.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqotdveu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dvszhihm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxkssxii.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfodzvjy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gkstskzc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htdhbgml.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kamkjjjr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfnebmwg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2txfsdcuc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqjtxvsg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xvpfdxum.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ukczygqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhjmwcnu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2usvjmwhg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2imandhbm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdimfuwo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wwafsuvz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cptluwqr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hrqyykgr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nxkiiyoy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gcusimfn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xdvokvkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nepxfwzw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kqsbmphl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cudpbowk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2sjlmbnha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khkpmwzm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2rcmxbrdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hoaauupo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ncqnqeor.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wmanuecr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bajzvevk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnufwqtx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zuvjedpb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cwdbtkwe.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2edzfalpj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yyojhkka.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fipliouo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywkvrzzf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2newspsmv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgpjcrdf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2paepfqbu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gvjbsgbu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cclcjkbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zzdnxvgj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpswijzj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cisitfah.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tsayjwjl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2stntdyrt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2okiatroz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zzemvibz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fglcdwng.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2yjvldqzq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pvsweqes.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2auojutut.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cidsqxcr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nxaxmyzu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kseybaia.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xlzzlnqa.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2olotrnbj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzvaivdr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pivvttsq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xlhuggkz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsxnwkmj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bkhdwilt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xmwibnhh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dlpjrjve.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nfyilagg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lgfbfsxa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mnedovnn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxxmpptr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fwldliqr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gcwjpxnu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhmztsyg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2obljgrzz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kccuzyyn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mxbenvlr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xqsmotiw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwyoeii.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbpvqcxc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nchdazlj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2quharvvg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cpziiwwo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tkqiudgw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yghjqwji.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dnhlxguh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tpbnbdrh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jztleotw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2meuhgpaf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fojofniv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2eaxdctqd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ejuxcpcu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2uzbgtfpw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2odtcddom.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2udljtfvt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzptfbjm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2adrriywm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zypxydnb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rkepkavb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbgwjrov.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmcrsmgg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gamzolzk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xdorojoy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2eumjgxch.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2chvorcac.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgolgzax.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kobygthe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jirrzsfm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ptyrookr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jpldbheo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nqepnmis.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fchsqzzq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ywggildw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ldhzujlo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wmalbwxj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bbuczfin.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2byumgbxo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xzibzhxc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xhqqtuax.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ztsykwdi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tyixpdeq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wnxibexu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxsmmlbn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ubuebyqg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjqfqxsy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rzvdcntm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rdmdtxfq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqtovbpd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2orfzjwdh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2umsujjts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ytkhqosx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbnbhdex.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtodtjtg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxuqlhdw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hefvvlog.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfutmlnq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jyztsjjm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bpwpiryp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2itylksdb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dytykiom.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qxbkqgtc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xuyfwcyr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qhlhtgje.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pbyzhcea.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2raboxmir.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vwueijka.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2swoxhtrl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wrplxrsd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2smlzvarq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ejmgvvcr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2otaostet.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mykylknz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bzoxqmku.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tldlhqpr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ofdevtaq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kjiatoxb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vlkzvtsc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbfpzpra.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2uvtlqkqm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lnereqdn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2klyebyyg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2oscirggc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lshffckx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ilazxyoo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mnqyjwqk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mzvcanay.html


<!-- 参考信息 -->