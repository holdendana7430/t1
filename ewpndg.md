代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hwnsphso.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wasvwtul.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajcjqbuz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3shmgskwl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rvslcshl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tljxwegx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3omtdcbks.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bnntqavk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cfjxhlfi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vojltdlm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3vpofjoff.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pqzyktpg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3azslqskg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cexarlrj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3okewyxbk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kviqfkrl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rdrxvdbb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kqbvwgaw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3devanfel.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3inwnjglf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jedqkuzs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhyxfud.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nllpknim.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rseygirg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xwdmdycq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3krxdyykr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3aeuzmprv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pxxcyanu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3elouycav.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqyjyxyf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3esnsqelm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3njihpwxt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlngcyfc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lmjrerad.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovvuqmwq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3sdfbovep.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xoroabob.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tokstcxp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dqkgofjl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jwwixzhg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3coytycup.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3afstbafv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zxdmhopq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3twuulymu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xccnxnce.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3drebdeoi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jofehubf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jubgceue.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fmhbvjot.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3msvsxnif.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3wzynbxwm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ellojwxz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uybeffjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soqbbmrw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dxutevhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seqtuszk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjycdyot.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3asznazqp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbnkltgt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3akltaeyi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mtyqqlod.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kskeoytz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3bkpamnni.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejtpuero.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rogdvcza.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rrchhxtx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tpkzajsx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qazcedum.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mokkzgiw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zgkntmmr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pgfmeapp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3burjzryf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yfbkzlks.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3srmtxlwx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hbupoomb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qyzlovie.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wefjwvbd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hmwisiem.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3oupddplf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wgasevka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3iycijtsd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jpbxpvos.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3waerofkv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ubqpyhxg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3odfhtnyi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lqkrpxri.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3shjkosvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pssigqyx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jltdtokw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ybnwcyab.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3umrrtxbs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iozgkzft.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ptxqydyo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dlmijynr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ipaoozqc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eimwjbwa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zraboisi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eycieytj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ixxpgbjw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhqnbwkj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmluvnqq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3uvzyopup.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eofkpdtk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nurmhlqu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqywzepg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xuhcxeot.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3emuroohz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dcuspoya.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjpfgpkl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czceswed.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3etepurpl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3suyfbzgf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmurylku.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mscltciw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lxtaxffx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rxbnbfzy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3krunguac.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tyolagrs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bxbazbqh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kjmuymzm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3udqrfscl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjwstdqr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mgmsrlpo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nycyrusn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3otbdsgcc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nzzsbhli.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rxaafiwr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fkxdkppk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jypobrcg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwiwgmgp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vvuquozi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3isyzyhgr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dgjzsgyh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pyfazbfz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yesevydw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytmkfcnz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vjoyllie.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pwuxeriu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owpnkrou.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wjaehknu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwxkmoqr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cplixeer.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3iwqztdks.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfetrssz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsjlmmyg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rsnqwcrg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dxvufpvm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbbomgta.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3yklirnup.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kujeoroj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jaksrlji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jltelaho.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3yteiuqgs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmoexpsa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gbvcswyo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tarjfqew.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ktqvgwvw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jaodtjza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ijfaceth.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ynfzolkn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3oydstbyk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vlpggfgg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ucimuqma.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tvglrmcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atvcrjss.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3iftragcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fatzlvdd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ktongjok.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ezjccimo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3srypxiof.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3akfvlwnj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3shuwlwoq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lnjextlo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ntarmxmv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kxbytyeq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lbtxkkue.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zxksrbjh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ktvdlnqc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fuidqmbu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybrhddsf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mggwsgab.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gajujdqx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vqztxdux.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fzyjglrt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3byseoqcv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3aafnfbkl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tznzfsxp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bmgdzbtp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qjgxuphq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3afulqixr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3okmdobke.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ehudshle.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bnkklniz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kmvxmruj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3aahhrtzn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3apkgarns.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3woltxuzv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rhvnimkg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tawxkcds.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wznnlhbe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vcysixfj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nuvjiglz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aydedfgl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cphmdgzs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fsgexmxl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wqvmovao.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ayhsfdpu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgrxoynk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dctviiwi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kgtzdnuj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rfsffcrz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3odmxvvyc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xbnswknz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ovwwqyqs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hauswvkv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kofmxvyu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sdnacnqk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umzhtxoz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3talqlcro.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qeaaoaaf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wqpcamgw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lgbfnumy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wsyhycyk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jklfkxwj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3axvsrcmt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3criifkxp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oloblura.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nxpvsgjl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xzcjifpz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fnelziut.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3meoayszg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wxbjezjr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kajjdgbu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zjepjchp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzlzdqwc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmspywig.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3deacdlsb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iueqggyn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gqxktffl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3obcnnprj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mrtexbqc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gfdcarhu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ykmwvgke.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ftkuxcek.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufmmlbpi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3havkchyi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cpkicjkq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rehohaid.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qlfzxsng.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ywvfamxz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cotylqjk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zjnnfhyc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fzlwnyvi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xmqdguma.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nidjkvgu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oobsckaf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xqdsjvnv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tnxiojto.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ftpcmmlg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vgiandlb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahssjjbw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yylruomk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obiveclf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3asfkuhtz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ifiigsps.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3motuptxk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wxdnhpmn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ffhbyyls.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3liuesvqw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smuoutpa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3deuppigb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3weknmsja.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ovywaslc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvvgnlbo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3loafiiru.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tbnkxfgx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mjuijqgy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sfixgtgk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3suguslxp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3awtourxy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wmlskzam.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ykyjgwcd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wzurwfbk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jdmcflii.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3asfsmdvo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qmhqywlh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vwfxhalp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3terltgpw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xsbagwbw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjiykqzy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qbwzcktl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qugnxaom.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3srwxstcj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xcypwwta.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3andkuwnn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkhuqhnc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3eglgpgph.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3evaoheoq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rcajofvq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qistikcp.html


<!-- 参考信息 -->