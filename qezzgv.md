代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nhyuoajz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dfetcrte.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kfzdgyqv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ypakvytk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3blpuxrzs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ahzwvdun.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3iqcwetnc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nuiklird.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ebtdkaae.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zsfsfdfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3okyfzclc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ydcmftrh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tjxiepel.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pfiagdug.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ylruolyc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qlquijhj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrytsjf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lonwgmce.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwbxcqbm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3igmwwyfk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cinzftxa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oqroonsb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ttdlrlgb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3eundyhfm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gkhjuipl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hqxcahuv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kclbdfmd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbhapwtp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkidcfxm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xywfrsde.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3irknunze.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3swwdycxe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vspygmti.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mojrmvif.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fqmtluws.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nkgxwtnl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dpjwtgqs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3eeoyfwab.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3snnyvvjh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hbttvqet.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cnsrlocu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3scepxkqo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ertxvvzl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3irxtfrfc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ualuqcuj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pajjwxpz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yhelzfxy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wrpvglcw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uzpinenq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwzjxpqf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pisganml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsfhcbpz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3dfjwoqha.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jbvrfuyi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3keodpurs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3kadontfc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3peatvpcs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bzgpocxn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jriwgypg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkemnhmj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jqiitryj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3otjpuhga.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ooqnzbsi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fsgozdcw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cbnbtely.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zmxonxaw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zgpqmmup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zxofcnui.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jdtsagph.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3axcpulrs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jzpshymf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3foeulsla.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lvqavvkf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tzvljtfm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3whwhgjwh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3btnvrzon.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmjxiyz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lfzzhvgd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bsvhuoxn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmiemgpu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ymlcdqfq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uakuypue.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3golyhivi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfntllne.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3byiokvtx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sdazenah.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uhdgtvwz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iwvgeebr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3abxpkjop.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rwhlrrlr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jyqzkqzz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wprzuecl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnrmhram.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xudqdncm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3avtrqcqi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diufldag.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lglhntpl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3asmyktgd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krwmdzsr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jtfjdyrc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3repygeqd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilmkfovc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zvrhaxzr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yriyqhqm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwfeqnda.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dwisixey.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hocviquw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jlmhxmmc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mprxognj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ithnxmuz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cimekhkf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mrbisixb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dijmnejs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sqpjmkqc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3igosxjvx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3nkkginvg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ernytewh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vqljqjeo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qtavebzg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3budxmhhu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lupkltuc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ccgsnqtu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wnaduhad.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbmpkvgg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zjuxrxff.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixljltdc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qwbwjpzc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ilctcvat.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ghoqnjis.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3czxvkmmd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yxyckogd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibbtpgkp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3qeitmipq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ikrntoih.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcxfadqj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eafjcjpe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itktnixe.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfbwwvgy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hlxexunk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnvuoqsh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfrmoumc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kefiurtx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mksnlatr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpwmmlhs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3clgposye.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3feekspli.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kleewyae.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kdiyfjti.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xnyhnitc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgbwpgwp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3amfrggjm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gvuuifrb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bytszyab.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nxyaihkc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kqfapung.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3smfgvmaj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zafkowhq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3uyiqkxos.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pugyemqf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vfnfikvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfxvgdek.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qjfllsny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyofkawg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3imuxlcnb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bjlstmjc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vcbmscvi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3drtpbsvu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gudtycxn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzdngwfb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zxgxxxwo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nkjdmlew.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wxjdkanh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wjhkiuhw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wmduiscb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yrnpjenk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtltxltg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryqodeps.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxndgemx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gpbrtsfj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kfyqigcj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ivwtoejm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3asptprab.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gjxgidqm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wnvfjsbp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vxauoorw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lbzhxuel.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3znktmvww.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ferzpsns.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xjuggjhq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cqvbbjvg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3scovapyr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rwdxrqxy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrdnmile.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbbtselq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbibyrp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnqcusve.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fcxmezyw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nqmvgkoi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dywslpop.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jmhcqizm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nljzszny.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzsriuku.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yclmaewn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nbpxbxre.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3drtyhtgk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3opznkdyr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fpnazvhy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ieglpmyp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wpmkxbeg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ylhrcnew.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sqpncwsj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3astfwqcn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vsmcmjqk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwydlptb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hcbpfryh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3picgknuy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gwqpcjce.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fvbxubkv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3snftdrzf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rwdqfift.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tuojvbqk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dsfvkdlv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdbqwipz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kbiwtzqp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rwspzuru.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pijmbhwq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3tztryqav.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ybvrkbdy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzzoktpp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3znqekyxs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3liipcwsx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgdrsamk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tjektgwz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3shwkyxmb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zwfuoqpy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bjczyiit.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uallcffo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3udvufdvu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3esfrogao.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lyhsmstk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uarbpkgn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lcaqvwvz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yarnddpk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3yeojihdu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pxkfluwf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zxhwgojk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zezeuags.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lsmzwqtm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3srykizfh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tlamjxuh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gzalntgj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fqoiuwss.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3senhzwwd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gtmsmdex.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3eyhvjzzt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bdkgasld.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjdgqown.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bvtivxlz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zjccldvf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rxjouxzu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ltftldlk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fezhzjhb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rohxhqki.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ngvmnomm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kblbqfeq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzarlpk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3chajgwcw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wszidmut.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lyrsurrv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3szcsxtqw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bojbspun.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gvazduek.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hhonzotj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eshdimkx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3asxuzomp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tgoucrij.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbntpccf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nfhkvbrq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3taonkcfc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jodpenio.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wqafgqks.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cpqzycue.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kbdaimrs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fvplfech.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3sljnhmww.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jofuuiah.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cpxfjmur.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nwnsagto.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xxfefkdu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mmwanrwy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nmwdaayy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipberbmp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3wrtyephp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3reckvpxs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dmjdwnop.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fvnjgmje.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bhhjozbm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3buqhouct.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gdbvnpud.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rcsgelql.html


<!-- 参考信息 -->