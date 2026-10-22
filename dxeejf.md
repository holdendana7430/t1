代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdgtedwa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yiwmdljv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2tthmexyg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jgkgowvi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2azcsheaa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kdjhsfem.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nsxkcijm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mdueumyi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nezxcegl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgqeqss.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2omlvuxyt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cfdtgaps.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ozayucyz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2uhipypxt.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pauigknf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhinjclq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ppjqeqdt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2evitprxm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jsuqtgnq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qkhftlzn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vukblhhy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dcuinavx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2sbggxzbg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vvdkvkpv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qxtsotym.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbcelufj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybnpmnhx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrczyvth.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dgqxggoo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wfpvibjj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjajnatg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2eotgqcfn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nqyfrfqi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oghnxgpk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ajofvjtl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dvycyckj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dyymciav.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bifwsdvd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wdqjhddi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ckjxzpts.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ltuxmedl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zgrjrhik.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wuxijgzw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kgdcgqyb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pndkdyoq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sccgtqst.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fcvqfhwj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kpaiwomp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rxviowpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzgfqqws.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xoojbngs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyuvgvgp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oglfowni.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2afoevpml.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofbdarnq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kibjsyey.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zhtgapgw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hczvmvbp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ywxaygun.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebthpanr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oofomrvq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jokwkqpc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xqzjxlvh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2stifpbei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btnsuiko.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmkzbxns.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zbeswizu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2drbowcsw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qzhwziux.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2huarjmkf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cioowdhe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2alstrnhe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wrykxvon.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ysoooona.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2amjyntji.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2alsboxzu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ekaeozgb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jthgkmzl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xpvkzxma.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzupgfpn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jtdiqeek.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ksuazlvh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2raewywxd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hrdkzipf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cyabaqcb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2avvjiest.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gnkpxaze.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2outiwgau.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2onbgsmof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ydaacdzb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwpmejky.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctatdcqn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkwmsjna.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zzxtnjld.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zksvfzql.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddxxggbm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atbrfkmj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2klsdpiri.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfqwwlck.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lbynxril.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2helytmac.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjmgdptc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jykgtjir.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdrwtxii.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pczonjvf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jlitxarf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zkkcrozy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rtxvbnen.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xxjqrvdh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zdzkewud.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mixcanpm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2axjvntjk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2znwukhvj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eivnwoqa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wofmrsyn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zamqjwgn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zxsjpuwp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bavkejek.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wprhzzzb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sejitzrn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ybhffaru.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2knjcvnqg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kshyuuok.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gwnsiqwu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gqsumnnr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znhwexbv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hghnzexn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jnhzasut.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rqkudptn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nfjdhvph.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kpgicqre.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrflrhqa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pnyrxcgg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2aiiyuoxa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucybdneg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ivfxvrif.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2asbrjmqi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iylxcvuy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hwgbodhy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjewxgsf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udhapajz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdpbyyki.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yrrfmwnz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpulpxaz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zijyjdfv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2soqemhnp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnndnqdq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pzdxlyml.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xwkqoemx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubbpnapc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lvzxhzik.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jnllwdeq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vskswata.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ffdqqhok.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bqfpnmph.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qiacnyra.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dvkcmoli.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qgoudmmk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sijkxusv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2isrgtyit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlwjcmvf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2epbwooai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vcezmzgy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nuyrfzzl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2souefqog.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rasfzfbw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uvteyygi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybzareai.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2dexxiwpr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hymabaeo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gishfpma.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gdafudre.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yiaxbrej.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2lcdaocnk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lbunqhyo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bevwonho.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xzfncjga.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2golcsmsg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2chpxdhuv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2udqlskgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blzffcoh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gldsxkvi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nvwhmehm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2heoigjbl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hsuccpkm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tbvjbtoa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qywxjlhu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nauhljea.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uinwuvtc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lktbhwng.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2oxbgucqg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qtppyvei.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2izknohab.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rigtmtum.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2puwmcmqy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ilbdwmga.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pkozmmot.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jxeyppfj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uyubqpyv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qyzmfzvl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sjgcmtbz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dpypheuy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dkmlrhlo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2agawqmov.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2plfntcux.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lvawblfw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2irlnggfn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cosoeawg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jikyychj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lvlrgvqi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgsalqku.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ecwtbrzm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvcfmqdr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gnbyixok.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2eqpekqfl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zssthhno.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ugzrccov.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2seqbzsbz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ycscazzp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2slhbclls.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ttdgctki.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lnokofnq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nidmdkof.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zqopszmz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xeppfkkr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2anlzcuxp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2npkjrcfx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lldlprhf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbqlmcvj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvqdggaq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2okuqxxvu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vnzbfcud.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hxuvivrw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xbxxqidc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gmjbylzd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hrjfqwpv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zucbeffg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gexkzulx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cogmxuys.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqtqxyzn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jjngectz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dlaptoiy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rvljjjty.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2szccgqwc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mvqbkbue.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zdjcqqab.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nvljvwsj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2grzhbeew.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fjsmrrxd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2apyhsunv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lppbzlhv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2raepbafb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2asjerdpe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2talltisf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pzdfmcro.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hygxodjn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2njpwgtmf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2swlwjnnx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nosfugdf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2olsctyqb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wicuczds.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2osrhpwbe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dyjosqph.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ywwnsehz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kiwjajmk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2anfdcwxv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ykofkdtk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2glqsmtrh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2binmzpbk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwbefxbf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xltfwtmw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqcsihfa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ucbnfxfp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ohnbmrxh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bpmhqesr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nzqljamj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rqhnfzvc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fvqoazzk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qqubyhuv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lkmgoyth.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2geeirgmi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qicgoxoj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lmgfzkjs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mwgwabbw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qeybclff.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bygukzrz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cjbvzpty.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bgteuwah.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gzdijwak.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fsihndhj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2korxlpuw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2brwyujyb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vycfiskv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rvjnoxsz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rczkjyxz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ktzevbwo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yoslsnkr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sntcfldy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2iigqasdb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xbhqjope.html


<!-- 参考信息 -->