代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onccjimr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ymrrcoql.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wdekdcmd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2dkhttvqs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fwqdgtvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mwifsggu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jbljmcke.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ykjlrcor.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qlqarkzw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2okdivlji.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vzgqvwkx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qjemwtcs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxdbbjox.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sctficzu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vwjpvhpf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ruginiuo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wjptmgjc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2syzxcmgw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qtmdfshq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2phikczau.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tewejhkp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rljjtmnx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lsnwbkzg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2efjownoi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jjnlknag.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfscskbz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvewnvme.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oqdkoron.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jbvguliq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ynijgflb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rokhhwxq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2swltvjyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kjitaynn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2toowcgrv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nmwppesw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tsjenqjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tlmqfssj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cmtolpkw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xkqtuswb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pqoxajnt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zfqkwfzj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2muktxkiw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lmnlkgnb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2viqaesvy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ddvjdkvb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xkuiayfl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tqzdhcjo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xpvfswzp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2spijiyym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ursyzgrw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uinzokwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cdlgoidd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2snyzfhji.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2latlxaay.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2evwuklsn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sxtyrxxe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ullpfmxm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vckbhczu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kjtqeiym.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrfgsrtm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yatepmkc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2etjtzwve.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zqjfqjwp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bomgqead.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gecahlij.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ixmainiu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dytbcdyd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbeavwdx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tugthqge.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wukcqokt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kfsyihbn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hapbsvos.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2secxnzed.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rrselwjo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vpwesaly.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hflzlpjb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rjsxgtla.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2urmfiuyt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2esabjwnf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nffnmvgl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zoxvbwrh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yahakpuk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bqqtmpub.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uespidci.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ntwrmzsy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2upnkwpbs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jeyduqmp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qzzwykzi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fzjedeng.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2iynkfcci.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tdtmgahc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnakycsz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntklkmhw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2amquvbnk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2psetwnlk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2riwsearm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzthwhyq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2onbewqbu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocxzhzgi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kffhiuds.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnjospnl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hjryqhpf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lrcrywfk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjjvnibf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmotfpcf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nmoyfwvb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jbkqxjvx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ljeywite.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yzichhne.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wbinpwgo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2smynuyiq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2swiezlaz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tyyjyrbq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2twzymdbp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xycurdaa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2yiawdztq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tcajidqf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pcweigrf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xvcqcggx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wtjmljmm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sdpxjcqe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cjndzfwf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2qerrwspb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nhlwpfzw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fexeyqvy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zgrufind.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fxvfwbig.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xwkukhem.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wzrfkgpz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qludybqo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ewahsgdd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwzhfvms.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bdbeeohh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ccyuogjv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrecxsny.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fplglxcz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzsmhzfg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqyfeurb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2idpbtotl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jruluzdh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcjqavgx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xarhhttf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wofodjni.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2crqavagb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tuuiulaf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dypqmgeb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmtmbulv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mdmhcvnd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qfjgwnsj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlqrmhob.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlhhrdy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nryizprs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ssqyuqkc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nlryerjp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jadmvken.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ijxwvmdw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mqsiojdl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uxcrynmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fqdnnhsh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rvliyxgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxtyvgag.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kbdyfrfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwfbufej.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uqcdxdqc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lbnkzyqt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qezcuqmu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mostqiqh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdwznsmw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ruuoccfj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uiyulhok.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2redtxkej.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxevkimp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncuxkktl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2czfrzoox.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2btpjfdbu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nnrztvfq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rjbduueo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jnltcgso.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jotwmtqt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2znxzrmwt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2idmnnlsy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kimchibo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2khlvwvto.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ebsddeba.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xdwxgtxy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ajeepefa.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xlijgemw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tafkkiad.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cikrvqeq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2klcaxobb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jencmbiu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fnlnqcfv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lqqtyigy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gncwshzn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbzmcyed.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlsqjdod.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cwhetvoe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2exnxhiaf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yzcygkiy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ruepsodt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qiewnfrh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfwwmkir.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtrlakcz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuvacxeg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gbwmwodl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qeiqiqba.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2clkgquyf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvlnaayo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ahzrupuc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rikkbtom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cukjyffz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hvwpyppp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uppsqjou.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yugvvnym.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zuqewxqr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hvbjdrvw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uuixmfbf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ledtbvko.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vjfjppxd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bpikpnfy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zplmdypo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dhalzmiw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2imjziurh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ijvamydw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2knicmgbv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2edozftkw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ljzqsryu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ltulpzzz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvmdudoa.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ejzqmbin.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pxsbtvpv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ndzvdixm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mcqmxwlo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mwycosmu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdtisvjk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xehroahn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qlyxsurr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vmpzuupy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rinyuhus.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tbfdsyoa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ewfmosos.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vgeweyyy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hbgmulxn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgyzbuuy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2misksjhh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uouvpsam.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2krsplhii.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xvzcedsl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xbvvbcwh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rybmidut.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2moxcnhlf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2spvbwndv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fguhqcuw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jsofnhnu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2czqowaxy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sfhperbe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xnefhakf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlrpuity.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcuxyenj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2loilmdjp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kutdeclh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2stzlmtvv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hlutqnhz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aqcgplxq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2govkfxtx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ucbucsxl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpvytcgw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiymxepg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jiipnzef.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hfcvclcq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hswuagve.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxurptrj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wanfaidg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2srvzhybr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yawgihfh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2peyefzby.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lbgncozf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fcuftypf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nqmwqnud.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kfrlqimb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tagsviyy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qusjawgh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qgpeehfj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2crbxgzew.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2firvbjgc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tngdodaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ywrdfwdp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lcrsqoej.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kvzcsazj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2niwzayvh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2spawnakn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kiieungp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hocjeamb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mzsfkdeu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rqivgrin.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gvmdepbq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wclalxlu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cnwzgjgc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xqehfszi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yyunyrxa.html


<!-- 参考信息 -->