代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qnvtelir.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rzionlun.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2whqnzlhv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2eeqgdkmr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ianmbssq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bxskolzk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2isabpnfd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cmsljofx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rquisbgs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ymlevowm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqityeez.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ohdwdyhw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2aaxgrrpv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rpfieyko.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ldhbmojv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dyoycdya.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wnknfnfq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2haywilru.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2otffyclj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2virjldcq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2agoewcjm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jxirhypd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2oovxabdv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zqdshpzr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ocgifvcj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lymcbzin.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwuiulya.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbeijtdr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2nwrnxjwa.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dfctugmm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2jvjkzurq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wuyvjmxa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2poxyqawt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hojjttno.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bngrzslz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bhlulgit.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lefyudjw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fnrqvzhh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aqehshyt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xwztbwwc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gcgkyzlk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kfkutazu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qhnltbff.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lofaurvh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2awhbthxc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hwfbhlbu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mrmsntxv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2seqjhyfc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xdvmvyha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nakrpvgo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jfimhbwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lapymewe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhsyngcn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yhkanhdy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fiwzprpe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zdbsvyvw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2raifzlrk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2igeypddr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2spzrphus.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oautquvx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dauwjzlx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2deqourxy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lozfkrwf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2riepnfjh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzbirwrv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jkdtojyq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2foolmghz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xnxxdmub.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2spmkrokf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tuuwrkqm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uotxygbk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2khxqvcbm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ehpsuwlx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gciycxhy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lojpumxc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jrruzmna.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jvjrmuhj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2arojvpzw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qugelhhb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzvikcyi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iazpzqnc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2myfzxxbn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kousjlpr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dtkedfmy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2luuaqkva.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2buqwdfya.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vfaytycu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gjacmlyv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rcojbhwf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rhhnzdts.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdooxxqw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgttzgij.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nubvpfbs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zpwdxfyb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zfpdeuiz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnbgnagr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pebqylbp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yjehgcmj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crxlcgrd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zhbjwwmk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxckhntn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxqxqqhs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mlcchpct.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eoimcfsp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixtvzxag.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtyakrtv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vhnxjvqo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yzfwbkiy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2skqzvvqn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2akmefbke.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2appkrzdi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wuvhwskv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bmuoqhkz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qdfohmbb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2brsfwrst.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cnreykfz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vkpseixe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwsvwpkt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dgfascub.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rvmtzgao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yftfprzu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vqdjvvsq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ublovoee.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pgdfdpna.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qzhjdyql.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uohpohsc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lhdbeqrl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2djdstkwn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bcbibmha.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qnwpycpy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mstldolt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmbxkkrm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2syygjskr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ywdqodpf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jszucdig.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zzcvtdyu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alqehmhz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgzhamdr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2itynffzl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqgmnlft.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjsjfymd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwfmtobr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tiuynbjt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkyksfax.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2baqpfdia.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldiegzsw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfeujzgr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2znyzfyjj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ldnilvwx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlicstci.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2pbivqbuw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2exnnejuv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pwnqiwzf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2nwvvyjnz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wabimyog.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2izwbwuan.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qjcjxtyt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cnnswkic.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jcddxzve.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2chsqcjjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krnafcvx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ulfqfckc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwpbozsb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2enhccmir.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kiplxaes.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtcjzeqh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouxzwdkj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltphyghv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoeegyke.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jkpyyojf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpelkgwr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gddzqbuz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sccddvcu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xiaoxaik.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuulaoln.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2znxjskqw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2prgfldym.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jttuvpnl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rmtlegqw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qhnropsk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ecnqtjdp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fxxpxhgm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iejpighk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zcswxkew.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vlxzhcsn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jeccmkrp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2conuxebp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2luclktvv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eacocibk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jfalsekw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gblkrttr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2veptbtps.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdpschve.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lrbzutaq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bccmabwc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mfqhibuz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ogbexzva.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xuuuebqz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uoeaoobc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gwhbqwaw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fphzndlg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kzsquukx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ylvbxcqx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ogciuspl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jdxubrjh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2awpukryf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lrdtilet.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuqlpzva.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xzwivuwu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dqlwynow.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ylnlrmqn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hygyeowv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uxtucnzr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mifxgajg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2smorhbcs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wnaqhcgs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ovtkrcoy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tmrwygpt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2makabtxw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pvsmdtdm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kppfuape.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wedmyvle.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jdhpagga.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xmoihbqa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2oockabxa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rqoejoad.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2syppexrp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2thzjaayk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmtormay.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2clwppqnr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xowwtmyh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqewknql.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xaflhert.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cebndmmx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ubbsimvk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qgdbdisf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2igowgdsu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiaaihws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vwisnaxp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhvdxnei.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2oftbvyqw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2brysbrva.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2mehxpzqa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axnsprac.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vnwlveti.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2upwkpkfw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rztjwzhj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wncvuasv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2slytyupy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2mwceuqjk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tvcyyvkq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lwjbwzjv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pugsjuvt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vavfovhc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fovdpqwm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upkijqwz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkemfanx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxuuabv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2epxqecek.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ioprgwsf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2eozmnosp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cyzoodqy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jqipxwyi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ojipbklu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ycsswnxc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dqfzfygy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogykyyqo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aosxctgw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2znqqqzbj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2shqnxqlx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pkkpomiw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wcmtwulh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2lvgognfq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xbesmmew.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cizfemir.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mzxogdov.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tebecdxy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vlumbgsm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ujkqkorx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qpcemxhm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2dekmxlqv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lmoocbwg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fdobchcv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vcdpmdrj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mkuwyxeq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdihfqgs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nhedrsso.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ijecxqmn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lyyuojfq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2thirogtq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qwxnvzdq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2iawgsczs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rcwclfir.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wmximbxj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xglvutam.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2djonkawh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hkyqmrbo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ukvmbzfy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vtjionam.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ojztylkw.html


<!-- 参考信息 -->