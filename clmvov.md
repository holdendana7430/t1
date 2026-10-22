代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezinmcly.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vaakhqqp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hkqrgeio.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2umanfxnj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lemyllpp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ebwwunsk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jhxbnzso.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pdxqzdeu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rhtpknct.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pguavycm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vwdxgfdw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ekvpjcql.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fwsomhsm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tqbuvqkh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vigthonb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rjnlscqt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wvjmijfk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dlwogwqn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2otnclmkw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xtbqzrjz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2uczxzdpo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hohofvty.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vuxbwgyu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2bxltaamg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vikqffzi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wnodlhyz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjvhguxf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iphmjarj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cuqqucaj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xuzdzgxo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hasxdcsz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qyzqvmfj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hcebsizk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lqigdurm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2muebzupx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2reeoplhf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uhmaphdm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ovndvkaw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ltncswuu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2udkiwzuy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lynkxdfv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqlauqgz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2irncbsvv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vuvfnxgm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2putfbsso.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2khbiiwwl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lwesayme.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fvychhbd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mchqhcwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvnkkivp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2itclwedq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvhuclmp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zfmnvxos.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nzsidgvr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zqwbxlbv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qiddxidz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jxvqnbmg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rweyrgcg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2yucpwidz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zccyfmdu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kevibfjd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2apmhdxwa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jciaxojg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qfdagdyn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdzgnsbl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2abfxjptr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2imthvmrv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zhphitid.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bypjlhdy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2lcgdutaz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sjfwgjvh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hwinbiip.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cnixmkty.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wxuisfdv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2alsyjhgz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bjejktvq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vnncxscd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ccwcalsp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zimxzbwk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cwwzuibt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qrtgcuci.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2sxoozscg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2umrxghmw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wyastnyh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvmwtmh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fvwljidm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzobrhdw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gkfxrawu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jbsqmqat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rkqkatdh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dydbqoyx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlhxvybj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fekjhdri.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aevxxdoa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dtlgnccv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukvnfmfe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axbdjlay.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxlteaou.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azqervnu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fqcjtadk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxgezdad.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2embdxnhu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fpwnctxj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qexsxvzq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cffwmulh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2seatxzcp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hnytwnlq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfzcebu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2docwnhsh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aplsubig.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vbcoazuh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2cjoddeag.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2skpbruqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nbcsoywt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uklleluf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2eefzbzca.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vlbngoyr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2mchpkbzn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2agufcuvw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ajbqmfkx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2btdzvhyo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rwrncyws.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsynxmn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wuiziony.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sxsiihpo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avmqibky.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rqjirfua.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2llesznrx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cezsrxyx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tlgxsozb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ymnvzwze.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxrxlhfz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2aukgcsah.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2smtyejtj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmzzbwox.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cdlzosyx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llhlgsii.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kraqboug.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2crcaovbf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgkqfrov.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jllcwttf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adqczfkf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2emjspzbl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nclqjspt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vzvrmtju.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkthevng.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzjnxipp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kfqdzltw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nxbetwvj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzqadgoo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wiiiwqlf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aoycyheu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2skulyuov.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wfriuopq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ckobvdey.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2azytfpxv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qwudkcff.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ohaedlfk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tidnbgry.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ccxojagg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxjvrgdr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2iiygjjhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqzsyspx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ufmxxyte.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tryyolqq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltppsajw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbcnxeyu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yshhltpm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2odarnomj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ckqiifjj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tlnptmoo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bcngiccn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xshmicjn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rgrxcght.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttkpxqtl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jouuojfp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkormbmh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkdiwvrf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2iykombyk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dlagcrta.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyfpgtkc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ducfolnd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gcvovebs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ashljptu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sfkqyvee.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lkxejhtz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kabrflsf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yaatkulk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vosolike.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hbeatghm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2eovryboq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wbzcemft.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukvbxlsq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdkgegit.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vmfeuwpo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ccstuaic.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zrkihrnq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ddzdbpuq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2asajacay.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hiodzpnk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yfajrpqj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2adyxvicd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwacfuva.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdpzeczs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxgadykx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jqycjhdi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qxdnrnpq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdjookjf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vrjehmoc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ypjblxkj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtxmogvs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mxhvjyjv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ydxcbxof.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cgbbbfug.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tiodsscm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2udvbeoko.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hefqhhqz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qbyszxfg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zfefknso.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bxgvyztf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xbioveww.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ydgrzmzm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ystmqbad.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dwmtlsgn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2uxqtfelm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2khxmghmc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eoxpqxaz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pmlmmeqc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwguxclk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cilseaeo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gnawonjs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cjadlzeo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2chisutpu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gjmnhtoo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymlgrtfm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2djaxmxnn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2abphdmhr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cihaoiqk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xsyltbar.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mmteeivq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hbfxfufi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2owruydcn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2eosmigbz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewzuuggt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cmitovyp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2grlxkqgh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wayakbki.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xmrtlror.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bodsnypr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rcbhouqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qqlszmvc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uhdfbzsm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pefcfvcg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gbjnflhz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fycuxxyj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtzardho.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kdarmkde.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2spymfpyp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icrgrcpq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lzswtdqg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uwdlwqzx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mckyamgj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pxrgeeho.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nnrfgqat.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ognsexsq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tuczoxuk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hduvadnb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fxwpheja.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2noohsrap.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qijyxqzm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ismcrqrj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wzopptqy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zovixluc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ltyjbxrr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kngeskrv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mbitufcn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ovuegdaj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xedtyyav.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xbidbpoy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nzwwyzqn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2muzrjccq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vewdzbsl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gsoxzalu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ddecdzrc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2spysndjw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqzltkom.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdmipbn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zlctpyif.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mzbeayuv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bdkaimld.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vbbilnrf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2apselvmt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hdihlvml.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wliigvau.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dlfyvvra.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2erjadqgz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cuwpauvp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zbribsvu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2thetcqed.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wnljfogy.html


<!-- 参考信息 -->