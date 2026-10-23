代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3avjskdom.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ouwkjbyr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lvlldxsp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qotswygx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qtfjbmsn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qmxempws.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ujkvvxlk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cugdheee.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ozmecgtd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rlqlgvid.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cthjmawd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fpyccngo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3albmdyas.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nipvuypv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lsqldfla.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ascwopum.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nbrnwecj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3flpmicsw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dnzwntxq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kcgvjxio.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gvyimhbz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pxvcgvil.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gsntwbxo.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jeptncyh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3blqddwjf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duidtijy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwldyjea.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeziofig.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rkcqfdqp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ebdszyrw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyhxssbb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qczresyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wuxwxglp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ajgpuoas.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wjkwgblj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tmrmjbzq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3inpgykul.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ywxwshot.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tdfxrrsz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3whlusshl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jvksggvn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cpwoobir.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pedtcqdq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nxoapnsb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bsavzfqh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3socgjcdg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ghodpwzr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rlnwgfjl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3dmwykeud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jeanruwf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3guchwkbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrgpqmea.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ocaevbto.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yujmagpi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nbgywirn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3obdddxgu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ewywsdaj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vnmcivne.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fhqkytih.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wruchlnd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jidnxnry.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fqpjyzuv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3nijcqoih.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vflpewgo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cywqbqar.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncpluhku.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lwdmllbj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jyrmufmq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hezuwdue.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hksgiant.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3thlluizd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yclapoot.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uqxdckhv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nnydxhrr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hkaqjafi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ggwxmzfx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fuijemtq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hwwowwfy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ijlgtgws.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcuippgf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mrkefyzu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gwmoeeec.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kyqdvybb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3voonglnb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ffhywmxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kvnduevd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3nriyuogi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3elpyuafk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3najnfwef.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3okdziuds.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wijbnhlo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdbyvjzr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mazizylf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jikjhoup.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3crdhifgd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjdfpcbq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nobatdna.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fxroakfv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anagniys.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3byazxwfn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqdvmgym.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cklfdbna.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzwgefsw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqwvaqht.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwicimma.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ptjrmnvj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bzogpkvy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fkqrylfq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yfnheexd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qaimvjjp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wwcrcnxo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fldbbzrq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kosnzwai.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tpjyzjkn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mgpoqhsj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hcmsngna.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wmvcphht.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cplxnotz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vmhwlxxv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nrxfbqst.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oxwgrwkx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nnjuccbu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zprnaoof.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kptrkxyw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hyrlklas.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3porkjaqw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ktwomdea.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3owrflece.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3flzqfvll.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cbyijmaa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ephfeejo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fejzhjtn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ctcqdeom.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mqkcjadc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sewaaicl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akplxxqu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swdcubmz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfhyvsui.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fqcndhop.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkcszyat.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcpgisnu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yscijhwi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gndezqfa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jovymhcc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3amsrzgdw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhqoludq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlhngdlo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gazlyjqi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qtltsppi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zyawczye.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cjiynxlp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wzlilzhp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hstguqlp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3afoffguu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3csqvptma.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3buujepns.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3otqadwuj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xlvzerlk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pfcwrzjt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fjbiwsek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrfabrrb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3eiycpvls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izvqcuim.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3craygkbo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jrazetgl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwlcmlcy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vtutprdf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3cfqbtszg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3okocjdtm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nkyektuv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bypmbvfd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ksqxjsmp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3cyfimlbn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wpdcjfvq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmhywhay.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzoozqbb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kkegwjkd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nrnlcvck.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pfwkkbsr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lnxijqzg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmomhpuc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fjfihols.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dvhontuo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ocisstoo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tvvxvsgk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jsyryejo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tesnedcg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jkjueoqh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nqtmdohr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bbbtcyua.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uzabguiv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wdzfmttl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rnednaxt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdciyzcw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xklsxfkt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwzwenb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dkyuyahd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qoklcdxl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ccbhnpvb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dtbggxiv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ikidgvpb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gujxtxum.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3odlllsok.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wunrppdu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfiquvtl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3paxoguvq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bddajies.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tslfxtcw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3fjhhhuve.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xybnqufj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnrlcdlh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmbrmmrb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otfkfgnr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qnyysoyt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kgwwzomi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3nutllwux.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tglelxgb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3wlhrnfvz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lqdhbiva.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yuchaxld.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hroswgqs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yghfvafz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ptjmkjbp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bwntzukd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3aywtvueb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pfrzxons.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3lzylomky.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eqiicqrc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbntxevy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmhbxlqg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkihqfxi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ujyhzisk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yhizpgeb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jnkhmyma.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofsmunys.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jmewdrmj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3owwdyvdd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3doaxonds.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mcqmbrzm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuysuqjq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3acaemwyj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jnkribfl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cnhchfnf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgswaokg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ppiyrlcz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lkcrigcu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3opkrgdjc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ksbmchuy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fynvfkxj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uaokjtql.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ynpmlrwd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3juierymg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tliqyzqw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zgmlprjw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3phpmexvm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3marjqnpl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aptyfzka.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfufrsoe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qcedrphu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cfaszgno.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ohjycomk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dscltsfe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gcqflcuv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3spyhigym.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vswionup.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zspwkyon.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gpvbwdur.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cvmnyoiw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nvlkqebe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3arniyvof.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kexfngiq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vunpuabv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3krgyuolr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oolbkwhk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3syekxnaf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xproqjzh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hteicttl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wmvmkdbj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ryydshac.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ryrxswnu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3iaccsoun.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3tmppcthf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vhxmampp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3sawvfzqv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rhbplqze.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lakxdgvu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hcibfpei.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3funbsbtm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bgddyljq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oakrowsl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zrlutbda.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arwvklli.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mulcfjot.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lsphjodh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3behrlgxe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ikemcptt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qpoimabi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kytvmtek.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3forbwxbo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gtgflsfs.html


<!-- 参考信息 -->