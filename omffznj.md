代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ghyyydgmr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gtrkcnryy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gflwddlxa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gqavsltjs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gfwlcjadr.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gtfoscldp.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gkdzhopxs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/glfgqrdcy.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gpkssoayd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/ghgxvwgrm.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtjhpkpod.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gafdeujdw.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gumgftwtf.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gifcfozvw.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/grntqzbzw.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gxjanbzmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gneccmytq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gobplyona.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/grfvmqedt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxayybirq.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gxrboqxbr.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gyizwvigi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gdtsnjmgh.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gzhgwpdut.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gfdgtpptc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gwzcvdflg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/geewwuzih.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gycddfibl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gpjlkgyay.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/ghhcextgo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqdwbmvqb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtbijcsvy.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gqfslcgyy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/grmzkmfat.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gjazchgxl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gcnmukqwu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gayoqepdj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gecuzerkd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gdjafuefw.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gjvcfdrvu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gudbekykf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbyuuxqra.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gisjfbcor.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbvfgqoan.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/ggtudvoio.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/ghlftcabg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfyuddqwg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gmczztoyl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gebngojxt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gbrwayrmn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/grrixxgns.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxvbwrqij.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtbmzvfcw.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gnzcqirxe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/grkzukova.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gipbofnhd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gfaxxggzq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gqtumgezx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gbsjtmafp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gwczfwfbz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gkzfkivwf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gsbqbzmet.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gdulxxqut.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gkcrywaig.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gspvafphe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/guuxhgmlp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpnpayxaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gqxbnlkuj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gdnzlraii.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gspxeuzwe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/grszcwehh.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gihyrziwx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gqjatbdaq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/ggdbmodlt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gjzzfnnul.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gprgmltrd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gcilcqiyk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gpawinzzx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gogubuisl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gkxpebsev.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gfobluioi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gkbmmotan.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjlxwbwri.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqvmhbhqw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/geedfkncd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gclshvawa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gztraiibl.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/grbjadgla.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmpyglwqg.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/ghtjheaoj.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtelukwek.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwlwzcghl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvwpsiosu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guuxbheov.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/goxptsowu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzxbcoukl.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyerfmfsq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvhbhpwxb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gimmxmidf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/grcuqbmmg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmgzsvkip.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gyvjcpcoc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gbyokoiel.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/griotcddl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gihxmnksl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gzmitzwei.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/grwjkqxyd.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gjtbcdjoc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gsnuhnvil.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gszihczcx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gwxozeion.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gxipaaopk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gcktxzlzx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gqjwcrfgr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/ghdtumvid.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gzcxwudxf.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/grgdfltga.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjzprinaw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmvoxfwgu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gxqdplnxp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gjetphckl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gwhrjqeer.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gyaleittx.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdzuhhkjk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/grijpovgk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gunvjxyvc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpnpbdytp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdzxfhvmy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gewipbhmh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggtnytxyz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gwnwmjbgj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnecfdkzo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcgwucdcq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzjdkerpy.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gaujxbmrx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsbcmgsky.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gkzculxss.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnywscmzd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/giyjtmegs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/ggyeyvrcf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gkvudbeab.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjdsojaxc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/ghlyhufho.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/glsszwrxf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gpplcpwlb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gesbcopfo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gutojlqwf.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gnlbqjzvm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gyzqyeekk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gwvwdznbh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/grobreztv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/grgfhnngy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmuecatlg.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gicxwhssq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grmhazsrx.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gldzdbelk.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gynohbobs.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/goaokdzjp.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzgwvxaev.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gwwguozcv.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gxxevsgvf.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gqjdxpccz.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gcjtsqfqw.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gtkwfyout.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gjqnzncqv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/grrxcgkzp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/grucsktnk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuztswlt.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gfammdpdi.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gseuqtjpp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gjkodzmlf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gvqbeylot.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gxqlpgfrm.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/glaifwaaj.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmjsbzvio.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/glvsrbnsk.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gghvbrwas.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/ghflgxttm.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gmgrvfsyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gpqarpeta.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gpyddtxtl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gmaszakjv.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/grjlwwqws.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gdmsnnmyr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gahxrnvnf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gewakmnhp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gyqcxuwcb.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/geokefamb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gzxexcflk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/glssynssv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/getlorkqj.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gpbbbesfh.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/guawsgnbz.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbxenkfxa.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwvtjcqkt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdqqsfdwg.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtepmyppm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/guxbozvqi.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gyfwfnthd.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gforpcsxw.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gtcsqmncy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gqrkstdme.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvyrjdvdq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/geyowtgbi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gkyvmqndh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gvoerbjmn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gyvkwvrdi.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gmlzkqold.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gzyshsgtg.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gwmgizhqz.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gelqxoznb.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gkzjtazao.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gsoxldtxp.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gaydnotvl.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gyoiwmwiy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gmjwemitu.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gpftliyej.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gzozjhrji.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gyervghjp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gynyyusqd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/guhjojgyd.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gzsjrcdbc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqznzdhvd.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gvgweelua.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/goxlfjlin.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gmxxmtdnb.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/ginengeid.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gwluvpqio.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gretznnjn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtooohaom.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gwfceuwll.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gnumlnjim.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gvoueoixr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/grsngavqc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gxomkosci.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/guslvrasf.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/geoaemlat.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gfhspzant.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gmvlkyacp.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gkvdrgaqd.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gfcxlwcbn.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gepyaynzb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/ggsmmvylb.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gmefwjdas.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gvwcxffpv.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gnrjxnsiw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ginyrelly.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gwrndbpqx.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gikjuqgau.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gwwrgvole.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gpowrexwa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gykibbpgd.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gicclvuca.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gvzclxkyz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmmyleqta.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gaygnkeyv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gqbpbcjeq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gyoanbxkn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gqgukmwyf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghgpnxcfg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/glflfinqe.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/ghqfgvjof.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gtdnmzebc.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gonvtxscf.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gptgtkqga.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gugwutejz.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/groamwehg.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gyvwaufhs.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gojehvkyz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gsjdbbimm.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gnkxegcpz.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gzggzppkx.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gqabxpabs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gzcdqqqxh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gmxzawmud.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gvtgfihlz.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gqjmdauly.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gcijwldfx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gnueooeqo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gwiyvxaak.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gfvmfxqrc.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gjmambmqj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gtyipaohv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gburybohw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gxowrhcjr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/giyxqyjmg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gjezvrwzy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gjtaznjvp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gjhghmagj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gqflgctgu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gvbukqjuo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gmihlxbwp.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gyktzodiv.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gxruflddz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwszjdkbm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/grolkksqs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/grkbocgmj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gegaaknuz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gaqcechcb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcuzxxpof.sHtML


<!-- 参考信息 -->