代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3njdjovuo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3tqsgwgkc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fimfjavy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3eijkzjdv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3opmfeqls.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gafoglbf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3uuceptfo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qwirlfau.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dfiukngl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkscbxo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ztxacbhr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zdxghktr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3eslfvcpr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3zcscyinc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ggidbval.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oaulqzca.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gsmakqfp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jejkiuzq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bsnndcav.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bbzmndys.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ycafvxvv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3bjdtbpdh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bilqalnw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lvaoxcsf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ammpegbx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dedpwqeb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gsormnog.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xypaeebw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hxqfatur.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qcfzytie.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojtndsga.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tghktzvq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hdjfcdsu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jemwjfao.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ogliyqtx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3latowbhf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xdwghkxp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3yzokfbbn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mjpujmdz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3toblcvod.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kmratcth.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3poekfdbi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3isuvxdgz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qdjjtikv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gaazghfh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fhextanj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3pjhshmqh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3phafxsmo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lrqxwvmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vffjublg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jgyoubko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqylvkil.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ilnsdodh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zlezumpa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ozklemac.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3djbtbzcn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ymhcmzpx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dyqzoyyl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xaaynuws.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcjiabfn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cgfkplww.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3asnuwegb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wlzkarxe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwbpnvrk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3roqbiagy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vwnpcbto.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3namdzdjt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3sswndozf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ucwqbjuu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bhrlyovc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3dblcwhhm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tytjymgs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ghkscuyu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ywgqhdud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zftpkeum.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vmgpoplo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qoyxgxvp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eropqqrp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oftzodcw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3lprxtdfg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vlnqabxn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3depirdaf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uigugsce.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wezmvyvk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rxsxvzkx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yxqyioap.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3efarldvd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zqfnefaf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ehjoieov.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3llagidil.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3loacvjoc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3szveigfp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwgvsxo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ikfiokux.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3nrsxpepy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bwsgjwwt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdiscxom.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qeufpnfn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsjhxxqf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pyoklmul.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhpwhnki.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eacvnzir.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vwglwmby.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3liqsyomp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stiytlet.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yoogrsts.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iahclxyc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpbftur.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kouzuskz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jfirmqhr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xuvwryda.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndbkoxga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ygqkgxof.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3trusggrb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3apszxdem.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bpuretdb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kavjjqwf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvduwzry.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hiqosvui.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vhzpcqpb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3taigtbzb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3znfnbnuo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vbqiyqra.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qiimwtai.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vowyissl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqcregdu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqsosjtc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lirneatx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jtjuhpef.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eizyrnog.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3euzybkgp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfpvmytu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gkxoqhmw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mmdjvhim.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qpsjpvxb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dloscytb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktryokqo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbsnrltl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bzkjnrjp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtfckyqa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkpapqbd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxrvctmd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwokhrof.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjpzilmm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nrcmwkqk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lsoeynfd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujzsikvg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ocgneuwd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fexijqfx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncmfuakx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3muukugne.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3qlgsaitq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3chnsdzlo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lznwjuhp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3insrgxrc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ypcxcxsj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xkhpixdv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3siaivzbi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pbrntdov.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3krfthhde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stxretad.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nbnwhyhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxbscoyg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gwzlxulw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wtlamvrh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lefqutte.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3avmrztko.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgmcwsei.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rfdsubpb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3whhwyrna.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dtetuhzv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzwzyhkf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jfpcfcqs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uqnwxdar.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdnwtixo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uexpnsgx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gxcvodzk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ljscidyd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3prhultqn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xlffynoc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rrtrdeqt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qakrtcur.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3skynvqua.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ovrnbmow.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fqmvvmqn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uycmljjb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3glcmfpcb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xgwjzaaw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lscsxccm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sjicsbpt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3innhtzya.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qzellfih.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ewjgrjxx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wxljbqrj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pmtsanuj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmtpmook.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3udgqogix.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tboidbcu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sdlkyhmy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mvpbibhy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qtmhnkgt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ghscssxk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bzvskpjw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fvdmtpkc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljfykdfm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gfrdeynb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cbxnnbez.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgkuixun.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rytdkyrn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hlgsndmm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nbmihlbo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwufantf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gajrmlyi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3emumrlfj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qoadkjtg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3iycwmrfz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gpwvqwah.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bgdvixqr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lvaculff.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcpmuxbd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3taoorvbs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kowziojc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ysyvpprw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uzogsjwh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cqsvcfgx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zuorrlrx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mrglxpkw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wiobmqrv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3iqkergof.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gifbqmhk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3idnjablu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pbkhnqaq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3sveevcef.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dclcshaq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3adcfnepg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bzpqtqge.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dzzyywbm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nunjwlwe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lwydkljg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cqixrcht.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bammrdrz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jxdkhyxc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bczbdetm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyoyivno.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3eazfivef.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dwchkpcg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ibtnwain.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pskthngw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dgfjhgno.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3btthohag.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jevatofs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hmwjqlrf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ngbzihzt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iggwefqz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3fbzhsqnk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfyjjrqe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pydosvcv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yiuisbhm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ugbvxpqg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qcxxwxms.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3swbjoxvi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3aaqfkboh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kyzhuouz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gauhabgy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ocebxxdn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgdnazkr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mpntyskq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xvuasadj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jkpnaaic.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yehcdlqi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iuccxnas.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdmvzyne.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3bkirkyvo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fnnlamuh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jiwuyffp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qymctxvg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3szgsywwn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zdasfnae.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hbiuiniu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ijyvkntd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3smrelclj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kpptecwh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hpldzdlb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3eoudgrbj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vflhdjon.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3oycpurvt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mtylouvv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kwvztpoi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uchzhend.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zysoossp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3josrqhwl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gumoislt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ymjzyqty.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ccgeostj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3slhswpkp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mvuskybf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mycqqomc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tksuxyny.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wlnwkzeu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3geyceezy.html


<!-- 参考信息 -->