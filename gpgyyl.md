代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3epxiexts.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vmcsxkew.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3smglkkao.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3uyxtqauh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3omnscrcd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yssljjyh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zpkgvdtr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jkmsyozz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjudtij.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uzltbowp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tnoqakzk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3odrldlpn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ddaekhjc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xcfyyaqw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lsprjury.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qvfpldcq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aszionje.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hzmuqnry.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3igntdbdx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vuixfmbz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jfxqmzeg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mlkkvcyh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3orfassul.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3bysjrfeu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bqdqkjam.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kfxydkqz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbuqiavg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nunfomnx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3apencwvy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3juaatmrq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ydqkwwnf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lkloesjx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qhxqjyrf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jvxdrfcv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ygegxkrj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zfhdajxr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ckosanpj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bnehmnnc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cggarkae.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bdtobhzm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lxpkvdch.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lyszrobs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qmwbjsxa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lmyndvsi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uqtqcbfh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sugdsqnc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3slppeqrt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3roctzpxr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vvwwtpoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaiihzli.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3oxjlcesj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsuprvbw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kusrwusn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xajjiula.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bjqlpuqi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3jihjorrw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mtzkvzsu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fyhiibdy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ypcceilk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrersbsa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3paiiznsz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnxpektp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wuqewits.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3grttpdnz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qcmioglt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tdastuyg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eexfvtyn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3kmucwejs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3hhfatusx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybgjeodp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tzjqmwyl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dmcajkoq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wxkaabhm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3janrnwdb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kzaerooo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bofnddjw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hrxbpdol.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mtcbkwyq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3brcwneyb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjfzbvet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lrvsqrmn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3oyimrgbk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tdeibdac.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jhjufgyg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zqxcuxfp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ychjesae.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jvhbecyi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bslehlxi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3iifydvgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3shuoenss.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mawibgld.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3barqllhi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alzermsu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oeyeamvx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3termrjnu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufneruxf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwoxwepn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vzmbdrdh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iixwdlyc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uowsnzxg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acwwyuix.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbqgtruu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3seapgfsp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfxilpuv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abfiysvf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwsoeuyt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3aaidnmpc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hmxntmht.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kcoahkdo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mqxdxija.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dntjinjb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwtylwqs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3czsdnszm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3soedkhot.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3fodyrvgx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vquvbxkx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gyfiojnv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucjtlfdc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iewmgkec.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jlnrhlwl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lvtxftvm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qldylyim.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dxfpykxc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wcttlznv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yyvnoada.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zemozdjr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfqzhgcg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3biqtmtxo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3midzpdfl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vtxlwcuk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3izbuihws.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cshaaljm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3buoanrvg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3szroeaie.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zotwtkvt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kevsneql.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atqtgvni.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfhcuifo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hdsftnig.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bamoehjj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bakebhst.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwrrnrxe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dvdbygsp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iupqbzkz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fipocuyb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpiqjwdz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rnwchtln.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wbhquchv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ukbhwbnn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bocjhkmh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3eoikqgwm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mldqbggk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ixdqlcbk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3esismlvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dgslvjua.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kcscrcmo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rlfrrpsq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3phmsqkri.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nmsnvsjk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xboraqii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtcwlhuu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3drwhjhkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqhuybaj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ajrokdrh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zquxgpod.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3umvwgbfq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3llcbcixi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hfnenctl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wodtjnwi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3oosvrfqw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxjzbnyk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvjzqlug.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tudrsyrz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ypgrrxhz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zesczhgk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3elwcksxb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3escjqeqo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uunsvsaj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kyqmffbg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhwncggl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ctzoimlm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iqthgjil.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pbxxjqea.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xqorsvie.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wlcvxnvp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fesvajph.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3llagtpun.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3udcqxqck.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rzqopotr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gdaiflqf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wpkicyhj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ymnjvqss.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ttqinqbo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qdkixrvr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esgbjgxz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxchbxaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ifvwcxjg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ovrqyoia.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ogidyeda.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gwduaavt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uiimufmn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmkvwuru.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ngdyhcnr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uekrstrc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlgqbmht.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dgpdhlcp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vnuvoffe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aagetdbv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hhnbvqpz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mmqeranm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogcnlkvd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmjuemy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvagycnu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gldaopzk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3abtgitve.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jnwfgfts.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kqgdolpk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hcdtwfmo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gglxgant.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lbsdxwon.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zedbfbsj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wnqvawot.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uxilmojl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vatarlpz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3umcrluzs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qpoxfnvw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nwtatvnj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hcenjokx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyuvtdtq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bkusfmtq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fercmtgu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzjvbbtg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3msvzikqi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzfqktyl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vupzulye.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3keomiror.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xjnndvau.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbmbcxcf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ttuefrvj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxrbgvpd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnorgfkn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mxwhjcyx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qwhbsqfq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3edqekyvj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ptfeissy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3pynvpgoe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mlcdeemp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3uvaiqccv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xnpxnccd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kfrywzrc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tbtztakn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qygeodgp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ypkywsly.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zcjthvjw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tjizpreu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ubytzpcc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rphxajuj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qgymckxz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsrbbcxj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3haplwsrb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tnrvpaec.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mhynrgxq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tbwzfcdp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ukihzsoo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hqyigvsh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3osmvejyj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gzdcrwaa.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zojwycyy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwvuxhr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vbsunbis.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3egqqeiax.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pjmohgrt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wuxhktpy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tmmvpswf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3naodveji.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nvmzybhl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oowrdhxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nlmpqlpg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3shbtilqr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wawvnmhi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xqmgwqoj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3skmnahhh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fqpfhyni.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rrqrtfqj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tlnttkgx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ytgvhena.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dxwjcngk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3asdgcgud.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3abunaobz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3oguvkpme.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cwvkokyl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hghkimha.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ddcgamwh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qngkvgne.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3fugwaeep.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3lpbrsshk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xsntkmbf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ybdykqkz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bupcdvrz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vmmidhhy.html


<!-- 参考信息 -->