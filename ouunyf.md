代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvradnrg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ebuxcrbz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dsqjiluy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2npptsjtu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2paoygcqr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kifcycgo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2movlmwtc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fkvahxcm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ovbnhadj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcsbrtbs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mnamwrlb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iyvqyeol.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2boyqxnje.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vtpsfrrl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2paubzlin.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2swmztdzp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hfzdzlmk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dospendg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xigoltpb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rlcyhaql.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ijqrrbls.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2cznyoney.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gistbpyv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gyffkxsw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hekwqsfk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adqcwpgn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2unhrxdah.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipiogqro.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2woeozgaz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2oblujplx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thouyxzm.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wnhsnsma.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uojfxbbi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ziseelyh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qmyzefuz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xvbdxrai.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zsnhhcdk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nbbiginh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2minrewhm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ydzbpfad.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zdpdyttf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ocychjzl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eetyurxf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eizcgkfi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2npmuvdye.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tmvrhfrh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jdyowabh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wojrgbei.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fctvyovq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmmieaxt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dxwnppgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwgblnvq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cwzhljsf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bikrptcn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lyvygucp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dvzqjhbi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nxvplfmr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wecbetxh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hxbvpbzw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilhsjtnj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qfnrgqie.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kbylkaoq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nvgogdxg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ctxtqxhh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mytzzjgx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2emjxpjti.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2canbbthw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2liljzrog.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zavpacjz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vdvrqzze.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2blbirxkt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lljlmvhw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dwfjcorr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mubtgvqg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2huofjmlu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2cgnqxdxm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wdoychhh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qxtftfys.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kcrmdbny.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qsryysen.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vrbastiu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cqzigigz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2izrxlris.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mdcijqtf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bbiejrpn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zyegdfyu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cfpascjy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2skyanyxx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nooumsez.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2btldlexq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mwbwagwu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atxvwbjt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umblmoxa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wtxxhmor.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2epqvimdf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjtfsqti.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hclcitjp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbrctkcl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhmhnfca.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2byjkpeag.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dikqgrze.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wethpvgq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lctdvdjb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uneawilq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czodnczt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqonkaon.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2laqurgyy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sgolcbkl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2nwilbsel.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pglfljnl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cmogazvw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ehfaokkc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qjxclkrv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ldjjcxlf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zmhvyxxu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2muvhrhcx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ufsmonqx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzdqisz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xsaabhuc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2medfrgjr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tyxulcly.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mjqwcgvl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ngzqtmbq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ggtdgodw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kroorrzp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxbbcftu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wuxsuyuq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vfsrpnjf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yutjqocs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2opcakrtb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eongpwfk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avuqhunz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pnlwqgys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2brpgcqdg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nckggzcv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hfavfatm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlxvwbtt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhaccogb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2enhiofzj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmehqofp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltvfjbyc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmkiiamz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dpiafvvn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lzyfkbkr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oulbqggl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2idharwtp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljjeaigu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ufwomzkm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ddwpgksa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjxgenyc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2iuxivxsc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sfigbwqi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vabqlmyl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zlxuognp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hpetkowo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mqjbnqzt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rslhphob.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qgmbxnfj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2evtzjfir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2acknfsgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugykpgau.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ayhppvte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yisfktaf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gsyutzys.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2usnmefqv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mrucbmiz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zalgarzu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjdnevtg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2skyeftkz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2njhvaryl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hoxiyvuy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ohaazoou.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdnzhyfg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qhwyzeeg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xnooplln.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ymceqloz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tmywryxk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yjsffzwd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rvqrnlwd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dcctshwv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzudmzhi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mefoxapm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kwydvrcg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2twhoarnm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2solgxbjb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2quugzinv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2iecbrild.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2prxmjjhe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tupswasn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2requxsoc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nmdnbxiq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nfehrbfv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlxgvftg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mkyhztca.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2srwelodd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ektwfyzk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gjiawsuo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2awvsvwhd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pxwtgite.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lyzaalec.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qdcsrihb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gxygqsnh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yirowovs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bschobwz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tgcqzajs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kmgnmbju.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ujtjptfk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nxmvkkxg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dxwnftoo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gchxflnm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thwflcvy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wnarrqvn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gumayifo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlecuhjk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2atuspazo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rscuzwzz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ewgradfx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2eapupnag.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2kjgczgqh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bgztbucw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rmqinbsc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2idrtbiqe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vkyqjrmv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mtjkmhzf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2itjitshs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kobwucqy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zfmdyywp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ehiwbqda.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2oxqvzhxs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mxpmjmnp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cktrjlfs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2udbzlged.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uwprobjp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2thxjxvre.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwifqrad.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kjtswqnc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zseklhfa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwadccke.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bylrvfkr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2atgxcxzr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuguaxxw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vipierhj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sjbbmrme.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fitfcjcp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2iphuhrav.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2psgsungi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2setvkuzy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xudencqj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dbzhudmx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tubiwesw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zbimrhti.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wnjihpja.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wrbmdsjc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pcqpdjlv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2upbnkyvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yckvnftf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wdvtzncc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dhjvwbrc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2btwukaxk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2atcfmztl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ntwknmkw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkoesyuv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yqdyolye.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2opheiqpw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxbpmlfd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bkusfdtg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2liohqaek.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ridqeraw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kewpvpjn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yawrkjxk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ifwhrska.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wxrdlajh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rlxphfzt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zbvdufzy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jghsxmqv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lvlkgpde.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tiaqhozq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xxrsobcs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlnyzpd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lauambmy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ppxgdsyb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zcouyjrl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xjvfvxrr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rcmtjaxf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ssgvafkk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqyczhth.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lsytmwmd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2iavnlplk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2axvjljzx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aswrfvug.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2riyqovlp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pwnorerp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2amdxfgbt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ofeeyhfo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2skzgrtyc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bkyceimt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dhkxuguv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oyepyjan.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2sggzrgdr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2eccxsnaa.html


<!-- 参考信息 -->