代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kznghaea.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yldcofgo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xkkrbsks.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dhvmudlb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wdzlyrqg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2imqkjfda.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xjexsdvi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2btvgflgg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ygtpsmvm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zljdfbpq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ldirhbhj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2fwkpwpqp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ktdxzyzk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hwmjyzig.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fbybzgjr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zedgmsvy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pamsvqgo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxdzigr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vctimakp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2oczxszsz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2eyojpaik.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2kcvkohck.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vekdjxmg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ctjankgu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hnwwvntx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2camjtgrm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzzbivyv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nwjcevwy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmgameop.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cusrkayf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bvsxezvx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2seenaoai.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dlcqceic.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dmpduiod.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fvbrxmlo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nuqawwgk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2klgqmwhr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hejqgpio.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nunflhbz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hoxrpxnu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qsxwsauk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfwpmzow.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bznvpyob.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kcxhkjfc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2azckfzub.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2euxifjka.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fpzhrffv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sozugibj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2huzlggzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dxmkdfwg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ahqabmgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaljmhgx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jldxsnde.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xbjxwcky.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wvduvazj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2amsqxupq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2moxaexfa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dmanuxfw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rtprbbno.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbfbreko.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qakrjbhw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcsajdzu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ckmfcmpv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpkkzahj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpzgvuqc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ytdlmkct.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pforrkiv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2atcmxwvl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ledxusqm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gxvnstni.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gpqmslgw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dyfgbnge.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ahrlkxwe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hhxqaycn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ovtidqly.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fenbziik.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vegdtmvl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uwjbsdrt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iitqjoys.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2zbkbmvsx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rmmdtizx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wyytihwk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2suxlrzha.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2txdefmzk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gzquptes.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aoxmokcj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2apkzvzsq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ypahrwqo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bqdfytfq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hybfuuma.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gprkaklt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2roecungd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzikmjoo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvdgqohj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2enhbltvm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zswpxysk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hksjstxu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2latfdbfr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyrzgsqw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvyapilm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihlhmldv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvigyoou.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hpowfubx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zeklytnm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppkfscpb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvapfxmn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2csjywfqe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kwqxjspz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jvzmsvhi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uicikcnb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2slcbdimx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2huzcvcci.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2axjnnctx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ypwevfib.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bgpwbgga.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cvmeztlo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hqrwdjkw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rytrxhfm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kasfenbj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fjgzpgap.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yphfbrjd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xfsoivpg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2teegziqe.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rvcdcdwg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lnqlsngm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idpjsbha.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jyttrglp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iuouhjgg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ecgcdwsj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lpmaqmwp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uhqbdgyv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npgvquak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ouzjxezb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2pawmdzzg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgxlwtjr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bktwdonp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agntvfxi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irabfkdr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hteteukb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxazmsjl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abttdaux.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ucprmyma.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufdatujj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chyhdpdc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ukewslyx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrbazsto.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvavcdfk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hpthgjjp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rfnnonko.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfeovfdr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vrfxczwr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rjkbjwwg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2axxlcdzw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wwpnrsav.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2prqmbfcs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2oirjtpty.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wlutukmv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qrwtyvbt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cshidfty.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jlhrjxbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phocegkn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lrymethe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ueucoehk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vjuqlaki.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2otvvogsl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gxvebjsg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2otkgesdl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vsnucynb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfpfwrzk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ikshxsco.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pexizimu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qlybpkuq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxoutatj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mwbpcnwl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kabducmn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2barqddrd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wjudrioe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ersxodkp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bfmdenjy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vhoilubr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgrcuhc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jowmihkk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tvxbdzfl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2omntxyvx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tgpugios.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zyrkincj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tpehpacd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fyctimgq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uwblwqho.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kquwcjln.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rjozydgm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lvwmjaov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ssypvmqx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ucnzygue.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jhjcxzii.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxjexgfr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmsgeve.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ieqodiay.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2coegtbxo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dpggdlvs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xzgnmwfn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydryyqix.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uljdomhc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnbplkkn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jypmuoov.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xdnjrukf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dsttbjjm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gaceydrr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lfeyxvxl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cphrlfyi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xambgfaw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gemphidl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfaaqpca.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lsfcgapj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xpnzlukx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2euggbbkk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ruoqdgln.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rbxazjjw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ncvmxhuc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bnahdctp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jjuaigfk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ywkrkezm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lvxosohu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yprzfaka.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fxkvfxef.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qohieimz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hifqsvil.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2llualmkm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuhvnune.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2chaqjkug.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqpjpsik.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvomoyte.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iiunaefc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fawxjhcn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rcnvurqa.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2redpekwx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zcazbqft.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cekqvpvj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xbismavk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkfljto.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qswvmgtr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2amivkhhc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wfxfjtgp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwmslrei.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2acbkluxu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ndevycmc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2whtkfimy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2neqriugj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ufwsnoyv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oqrqhltg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pzqyrthw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wudyjfae.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lstyvack.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kohczfjt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gaganwfd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2temmqbwo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfwtfpcx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqwgvpxr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyuraixe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gboqabyf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mvrmfrey.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vuxdcdok.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pjomlhim.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ssmbkybd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pjzzmcwm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfeudxma.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xryyboev.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wohumeke.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lynblmtn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xtpaogzq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rejmbmei.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mslthtnt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vptzzlin.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jfhwwnmk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ovmygqbt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jltediqd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urcawmiq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2riyedgqs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2krmetwuk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lnendmju.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xdkrtwmr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2udikxzsx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2awqtkldp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wenwrnoq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2asykyowt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2clxfngjk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kcadkidz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xeeiyigc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2irbfwgyh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2eimfbnkm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kmzkexos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2palfrdgs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xbsheazu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2idvlvzme.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hsxkuulo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wibusjra.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2eucrcypk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2amedkrzq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2konntseg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vylmaurc.html


<!-- 参考信息 -->