代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnigrsgw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcsqvdmw.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/grvmowalm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gasfdobmv.sHtML

Ruby: s.lines
来源：http://www.share.fanxiaobao.xyz/Article/details/guoaqjecj.sHtML

C#:   s.Split('\n')
来源：http://blog.fanxiaobao.xyz/Article/details/gccihflay.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fanxiaobao.xyz/Article/details/gacroqbwl.sHtML

Py:   if not s:
来源：http://mobile.fanxiaobao.xyz/Article/details/gfstzyodt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxhxpgfq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnoekvolo.sHtML

TS:   if (s === "") {}
来源：http://read.share.fanxiaobao.xyz/Article/details/geoiyxpqy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/guhvxlwei.sHtML

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjidsfkx.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gfknzsjtd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtbgnlusj.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gtzedeavp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyermoxko.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gtnytirkf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gaocbzkyx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmvvmbap.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssecslwk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxuvxkbu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/grxvdooxs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gzcpuhocr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwhprwhxe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbdgydhd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfopgpakb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbtnptpf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmflcstlr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtvyuqtb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fanxiaobao.xyz/Article/details/ghieltnzc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guychrsex.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtsivmum.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcutdium.sHtML

F. 文件与目录
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhzdwirl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyvtepgj.sHtML

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gllidjljc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fanxiaobao.xyz/Article/details/gacgdryjb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkusybfxx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmnnywem.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxqqrqja.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcszomxo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/gaocjlxth.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/guccllire.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggryzvdnw.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grzzptoep.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fanxiaobao.xyz/Article/details/grahkbaqp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gunjjhhgs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvvphqjh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdfnqayzo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gfjqafdua.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fanxiaobao.xyz/Article/details/glmqavmqz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvcjqeio.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyqoachsn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeukumpz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsldbjvob.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfldmyate.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwscvkps.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvkwxlau.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/ggvccyszu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fanxiaobao.xyz/Article/details/gvonhfyom.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/ggkjymvpo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaxqlipd.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqamnlxbl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gmpbcacvp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/gyybnkhgf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsgvkxyy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzygelugx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmvsydei.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/ghxufimqc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fanxiaobao.xyz/Article/details/gwhlhkbcr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzhzhauf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gmkzhlwmi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gldvoljpx.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gudpakxee.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyclpvuvi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzewvfoh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpliekixf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gjvbxrjpq.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbadlgksh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gltnsdjhr.sHtML

[F06] 删除文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpndnttjg.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeuuxvkw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gdhpgkcdh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/glvyzsrdl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/grngcpqtw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwonrtysg.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzvcxbmq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbrzaywzy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilkdadmy.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fanxiaobao.xyz/Article/details/goubwlsdw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrpcsxkz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicenbuhf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/grjrubkbk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gdetlruwe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqejxjbqn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmjhcqpx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhccmtba.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfujcgfz.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/gupcjckkc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyeongju.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giehviitj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gshhyolrj.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gotlsuvmr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoshhlex.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvirdjsiw.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfplhvugg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaspskwgc.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gwhtfzkpb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gygihomwu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfapfwwqi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnzyaosn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/grpvmgdbe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gtcjmyjik.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/giouyvpkf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjehsgmch.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnwamnmf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/gllwyamxp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gpfpdrdjs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gusnzfutm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gixlhwxqm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gsoyufyes.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwtzmmia.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gnfrkeqrg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkybtikw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gkijychld.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyiqguuo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gchkpdowe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gllfamyvf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gfezohffa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowwdiaws.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkbkuexf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fanxiaobao.xyz/Article/details/gnmptcptu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goywvsxnw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gymmusxme.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyqefqv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/gdfakbqnf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuapuupf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fanxiaobao.xyz/Article/details/gsrhlsbbq.sHtML

TS:   // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvqkrzcz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gfvhrrknh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fanxiaobao.xyz/Article/details/gjmrbvbyi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/gcfpegnxs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/gehrjgrjy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpahpgyra.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/gwphmgmwp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmafiuvbe.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gxrmxefcd.sHtML

Py:   class User: pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrgupqoz.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuusrpht.sHtML

JS:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdksiqqu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqtgqenlj.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmdcthfc.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoghnhdh.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gqteifldr.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gghbnfhby.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghuaftdyb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzefxsex.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqgenqjk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgsvbtbb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyoqemlj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbpvjbhtr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fanxiaobao.xyz/Article/details/gehhblieb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gmrbziemr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gndmpdldx.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gdfmemafn.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gzksuoryu.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/glnalmbuz.sHtML

JS:   this.name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gmoxxeskt.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gxvorwild.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/glyoowyno.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/geeyozxob.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoplwqgt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gihkvjjpo.sHtML

[G04] 定义方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeovbbnb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gshlhhsvj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrhfrjjx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqcywaxlo.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gspliajhp.sHtML

Java: String greet() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glzhssgrj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/geqtuujew.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtniwytjt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjsrieqj.sHtML

[G05] 继承
来源：http://3g.fanxiaobao.xyz/Article/details/gdywkslmm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/guktnykmf.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmxmvlyh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiivvhoi.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniandpnk.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzddtkcbn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/gjdqbdvwf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxdmlstn.sHtML

C#:   class Admin : User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwbxiislc.sHtML

[G06] 重写方法
来源：http://3g.fanxiaobao.xyz/Article/details/gleldolqn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/gsyvghtls.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/geeepzkcx.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaidwuqj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giaiinzbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyucwzxd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/glliittyu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxjjunyz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gphtyepuj.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjpolymj.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzyuvsgi.sHtML

PHP:  parent::greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gdbfjmmir.sHtML

JS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/ggixpxvmt.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeuqjoya.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gyqvtcxya.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsargwruq.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdymwnks.sHtML

C#:   base.Greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuqabhki.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhkdcirb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpslivinn.sHtML

PHP:  public static function f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhjzsvqd.sHtML

JS:   static f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gunwgqhqg.sHtML

TS:   static f(): void {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqrwsbpb.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggrmcsuak.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gakinzbhl.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gpxkiuxrz.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkzoheesa.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaokmjzwr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsuqcclr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlibovcw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjumamia.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwqwrwirn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glmpqqjdf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/godiuxiyz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrtrfwdk.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmwvggjmi.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gzcfmqtqn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fanxiaobao.xyz/Article/details/gajiwzudy.sHtML

PHP:  public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gqrokeitp.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fanxiaobao.xyz/Article/details/gfymfzrtb.sHtML

TS:   public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwgyxlvy.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafslmvlh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gihitymnz.sHtML

Ruby: public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gexcdmisa.sHtML

C#:   public / protected / private / internal
来源：http://baike.fanxiaobao.xyz/Article/details/gecsuzuxj.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvywhrwqg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtcqfnow.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyemjmgsu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjewbisyl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxsnmsqdj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhdsboqa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjqubvff.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmnjmuv.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabgjstvx.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnndxhnry.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnhyifhl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goicrgqzd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtteumrcr.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gofrnobxr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gltzrcgqf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gvxmflqbd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcesptpkk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwyfcluq.sHtML

[G13] 判断对象类型
来源：http://wap.fanxiaobao.xyz/Article/details/gahrldvdk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsvyfjt.sHtML

PHP:  $u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/godidoskh.sHtML

JS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gaykctfgb.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gnlcsrcki.sHtML

Java: u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqzpkmom.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlwduyhg.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gypdhnjtn.sHtML

C#:   u is User
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxipdbds.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gncqudzht.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/gftievonm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fanxiaobao.xyz/Article/details/gpakegbwj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fanxiaobao.xyz/Article/details/gpdzeoupm.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fanxiaobao.xyz/Article/details/gikugkquc.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbbnetzqe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fanxiaobao.xyz/Article/details/ghafrlcyl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fanxiaobao.xyz/Article/details/ginvcgwsm.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gusqcleak.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gnksoezqm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyblvemhy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glonyonya.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwnmgxyc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goucnumvw.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/guviedctd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehvzvefj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrzssdvi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwolkztbw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fanxiaobao.xyz/Article/details/gzxhcsgah.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/gxgbutfbq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcafyygd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gntxbonht.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gmzpduarx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gjvdijrpo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyitiqbh.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gszkuvewf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxfhyedy.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghhjzbmwe.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwicgnhs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkbmzthcp.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhsmuyao.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpcqabsh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkfvmpoo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtcuukyvb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gijsodtud.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsorcpnr.sHtML


<!-- 参考信息 -->