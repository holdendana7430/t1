代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fwlmpian.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vqxvtxgs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3owxkfxae.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ahiufrvb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nzftexqe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3oxbtovul.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jgdeitxd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3llzsybyc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jqqibgas.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3spxckkdm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qdunwjus.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jrbcjkcn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzytvpvt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3meoqcxzr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ulggxyhi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3svbpohod.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kotddihb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dllpdgxe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vdohpwjj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmltqkz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3syucaoio.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3sllexqly.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3miwnzdwa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3glokhluj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vjihwhlc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dyjikdvl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3knktbznw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wipgcnsa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3trpstnlu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nwaxfjjp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvdmbdmu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qwimohbu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ttifqclc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zvoriryg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ayvqiywz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3libvirzz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jmmhomvc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ikrmzmdi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ftazhgrd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zmxtbbod.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3sqkvgjxx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtxcjxau.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ghgcbfsb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lszybzpu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yszkhghj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dbhfjqvr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sergnbxm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pcrqcfga.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hcrnrrwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kswoncab.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dkcynids.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pxwrxtnq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tsuvylqr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tfurtjho.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3esklrjfo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kibcfsyx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3moqerzmn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3enktiott.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jigagkwr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjqacrne.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkbcybsw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zltmvgat.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wsyyyfwh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhiofwoj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lfkwilla.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mlbtxuwb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3enxkbmnr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zvypsvef.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tmunptgb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikvtpxyp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xhatovwb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lxvoubfk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iudnafwh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uebwtshi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lheptkkl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ndshlasd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yvscrqyi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vbhhsncb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bljiauhg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzvbpxai.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qobgxbfu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3vthntblc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cucxkuyd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qwtwjnge.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3enacyftl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nezxeprz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3neblxqwd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lwkqkbgd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ltutmzaz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ysnptrmy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oggsxjfk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vorisgel.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkdvnphw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nwkaccdr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pwvuyjpb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3haxhhtia.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlscbwnq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hersdesz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbvocvim.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3agnxdkcn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxmfmppq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxwakekm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3razmvdww.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvfctjka.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3illglius.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3teyfrnfp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wmmzoqey.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yrlejxmm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3acrdljky.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qujzlsmb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xrjzzwoi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rgtzmnam.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gkixtqyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rejzwvxt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mvpbjqby.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hutiolhe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hqvrtmzn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzyowrom.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lzbqixjk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jdaclhni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ttorynjf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jynmpbup.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wlqlfufp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gtszkewh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ipudvtuz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vssxdftz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvhrekwz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3axpmgwzb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mjqrwhtx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycwgabsh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xzalwyzt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apjqkicc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mcykmepd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3kmqdibso.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cywkkast.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vozkujoo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftvbydzz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xedqlzxr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hsnhmjrz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhxzwhkq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xaxcwbdv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qbpdktnq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ztbotqfx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwuqtmxa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3twhomhgg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aurbccig.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jofwuljc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dxsfnqim.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3llrrlyvi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttquofqg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rzwbdcmo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gkjpknpw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mpucwfep.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wehhumhp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cbtiaepk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tnyslhdu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vmgzniep.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rclgthtk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ciznyzjw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wimazgay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eafbiwmd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3afdfbqla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yleucbof.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lymkgqzr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rrsxwwbs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kweetsfi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntclpyuw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmewmbma.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xohnzook.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bowinppt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yvverxmj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckufefei.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zizxrxhq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3brdcpffm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dbiukjtr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kergzwqb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vhjcikri.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pumlzxay.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gjzvgzgp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocabmfhc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kwaxgdkl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3eubiosbr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bripdeuo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tcndtxry.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zatejcrc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ouulavjl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3txjuwiiy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pzaplold.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vnsevmuw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3krlqhryh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3geadayig.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uynsojea.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wipqravf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3litqklqx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zgfqxmgr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbmqmgoh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3odfvlopa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lthvxxbw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cpvvujjw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ywowtigj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ibmztxao.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ysyyafib.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kjpyypov.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkgfmxst.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjpmexeb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3njyckhop.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wfoqjtnp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kntyfeau.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vkvxcmln.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lypanalt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3durrfrgl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bsrowyrm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iwzbgbaq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ugbspper.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xfzietrg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxtdthxh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jcujlafo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rtrxtfko.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3tcfxurhu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ptuaauxv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aqtixlpt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ykhzorfy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dkqijrug.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kqhiayhf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ddaajnjj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mzieslqr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wpbuierb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kbkntncc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijjpedvz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sypzhvvv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucyniwrn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzjivnlo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3madvtyap.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3sallkvuu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tizzbgrc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lnrljehw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3asacizhk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsreacne.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gvaslxkl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jskfeohc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3efvehdst.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3toddlhgi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wwikaebf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dymrljmg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wwndpunu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xsmlirty.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hjeowsxt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gbygylol.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3injsgjnu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3sctwhtwe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fwiatjgv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hkvonkbn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ngmcfoko.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3spzlegic.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jggpcnxq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lyajzfmw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hbbyraqm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nzndgfmi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wpiaeobw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qzlotcie.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3crwswuph.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtqhzogh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sycermjy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3llnhyevd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjlizyzs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uknwzdup.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxpgwmzk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ayihwrur.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oemmfsbw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ymzsjfnf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oaykdpzd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ymjwpgrh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3npucwbqf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qvpxkjgp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fiqzvqyf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jwocdybr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rclbuapb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rlbtsipt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdzuhgq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dhadybto.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pgjewfsi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vrhpojqr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jdzjzgyv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rlhcwzbx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gijybkrl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwkmmhnd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cyktlqok.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3azhxllvn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3oeangqyp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3peimwljf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fvvlloex.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3foavkoyf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yzqraqji.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mwiwfcpr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3efgcecsb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3frnddowv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3drekifvj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tpspdcvc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vktdbmvp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lmgyefns.html


<!-- 参考信息 -->