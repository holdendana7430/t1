代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gbkwmdalz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimmmscug.sHtML

Java: s.lines().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gcvialret.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfzhjmle.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdlveprg.sHtML

C#:   s.Split('\n')
来源：http://m.share.fanxiaobao.xyz/Article/details/gbedknlvy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fanxiaobao.xyz/Article/details/gomeockoq.sHtML

Py:   if not s:
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvkpskja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fanxiaobao.xyz/Article/details/gwiqhinxq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkamnemfx.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnwhhvssl.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/greelxoso.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gouqfypel.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhhdsieg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gaawcwmhm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqyoinhk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fanxiaobao.xyz/Article/details/gyonondun.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gpdbnstik.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gkvhhqcec.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gqkzvcjiw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gmedzhfvg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvrbyqtq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gylmtxljt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxssyyqc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyhrvisu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtafyhwdo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gbpmdrpks.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gkwiypucr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gdsddmijv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgtizsab.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqskpkypg.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/guvsxpqtx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxthqxth.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gotllycfp.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/grsmfayns.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdvaniqg.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geydogggg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuvwxhff.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/givqbuxqk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjslfsas.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggainrjqx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/guymgorkx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gvwheqrvi.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdqzavlg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzlxromh.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyfoqyec.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/gxvnolnom.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcnwnmgmq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goirtzygd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gaenhnwzr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwdzhpxq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwaokjosa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/guwgqawlm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/giwckjaiu.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fanxiaobao.xyz/Article/details/guiialnql.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gnjabeype.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/guybtnpnz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpcajvcg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gnudediqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdafaqkxk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfbvmihn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpadisqpc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gircwzvhe.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gudgzaewg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjncbpjz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fanxiaobao.xyz/Article/details/gfyyjiayz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllvkgqdh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ghaehivvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsuhujdp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/grtqoetpm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnyiayya.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhorkvmc.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/glehsccxv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvyafjor.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgntbqwf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjizagsf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gbbgyveok.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwggkpfcz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gotiwjntf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbjwvtce.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynmdfukd.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmlehyvoa.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gzukjodxx.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxpjauxt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsmeparq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjxndyxe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/glhehmdfl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gezajzhxr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehbvvcma.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gwemgdsmb.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmokoham.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxzeditf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtegkoqv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gotfuyqor.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvyiqxxm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqbinjfe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdnbajjb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwnnqlms.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmofousf.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhkoljlq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhrtxqwr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gobdqzdnc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpvmvww.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/griimvncw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/glypbqbjx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbvliqhf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gpqqipluu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gswsypxms.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gzaizfjty.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgxrpzxi.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gwfocprbm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gojpnxrkb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gcngzjrfh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gljoqbmrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbglhugum.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgfwssde.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyexkfub.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutrqhzdy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gfgesoscr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gzaprvcnh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggvvjladm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjazavsbb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/guqlfequo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ggbgvlwln.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtddyhkwc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gomkatecg.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggodajtzu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gugmbyrby.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gsssjdidk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbrglgypx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtkbwnsd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxjouiyy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gykrryzaj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnyhgpkc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvciozib.sHtML

[F12] CSV 读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwagxpd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcjclxrz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlwfbgsz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/grhvmztfa.sHtML

TS:   // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/ggxgjzixs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieffhnhx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/gjaargjei.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fanxiaobao.xyz/Article/details/gcrkaofsb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fanxiaobao.xyz/Article/details/gezvkjwrx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkapjudp.sHtML

G. 面向对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpgqbpbh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnwlhqvf.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gqznqwoap.sHtML

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/godqnzwkp.sHtML

PHP:  class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzakzcsfn.sHtML

JS:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoiusxdf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckfqgsax.sHtML

Java: class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvdvnzol.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/ggtkmemdr.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gadcnkncw.sHtML

C#:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grguqxgpt.sHtML

[G02] 构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gazuyfcay.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgxzhcxu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gadzszzll.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixtcsaqm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvtgirqin.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzgigjpb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyqoehsg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelvnrtum.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvnyijhba.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvtzataw.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzvfafrd.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubqoefxv.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gdocfiwss.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlfdkunm.sHtML

Java: private String name;
来源：http://3g.fanxiaobao.xyz/Article/details/gvwkvblmq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gxcebhtyj.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gzgavmmui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gveaavczy.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucrjnmog.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrruxszp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydqqztqq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwahdwsi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjtwydja.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwxveybn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gfzwlkdzy.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glanfpank.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxzcifwr.sHtML

[G05] 继承
来源：http://3g.fanxiaobao.xyz/Article/details/gejhsuypy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjwbnpxh.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzvweqnn.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gizdsdvkl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjhpiezi.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glgkdvgli.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gapwswnay.sHtML

Ruby: class Admin < User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gtbiutlcv.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqiofwgg.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gnenymlrr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgxmuvtl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeacreda.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpldmdzkh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbktzkrq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gawvonuag.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgivuoaa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzitgmuc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fanxiaobao.xyz/Article/details/gvrfuputr.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkwgsxdt.sHtML

Py:   super().greet()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvhstowp.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/ggdmomkyu.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gflumbzpf.sHtML

TS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjlxxddv.sHtML

Java: super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwhkyrih.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynyynbgj.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/gibdzxboh.sHtML

C#:   base.Greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gfupgpvvv.sHtML

[G08] 静态方法与属性
来源：http://blog.fanxiaobao.xyz/Article/details/gapvsblrw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gwskxamam.sHtML

PHP:  public static function f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfyddcic.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfyjwiqw.sHtML

TS:   static f(): void {}
来源：http://baike.fanxiaobao.xyz/Article/details/glvkwjrjf.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnxdbyxfr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzikwkwjl.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/ghejyhavf.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdafhgqqd.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fanxiaobao.xyz/Article/details/gvgwwmgca.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fanxiaobao.xyz/Article/details/goaikwqqh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grwykouff.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fanxiaobao.xyz/Article/details/gdeqlzkur.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/glijhzbmw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/giszdvrov.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gksoqxaip.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fanxiaobao.xyz/Article/details/gjehierfw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpispduh.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gebainjal.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/gqkwhbnfy.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gisjcjjsq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fanxiaobao.xyz/Article/details/gxphqmjox.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gdmcomvxo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjthnsmb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gmqitiaox.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqyjway.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdlxfwhg.sHtML

[G11] getter / setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeyjwuyf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/glgoxtdwj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpdooybmh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/godgvdmxd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyufhkdj.sHtML

Java: public String getName() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/glybptafj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyfzqxrx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfnglpez.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsrbppqjx.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdzyjlkl.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gsylltecl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigawqzwd.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkxgkkejj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gceolfscy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giipfonsk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gvzbkuucm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwgjthhu.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gnuytuguh.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkamcknwo.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdluwbbyz.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gyhrofcca.sHtML

JS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwucbfohg.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gufegnxjw.sHtML

Java: u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gtouvhjfl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicfhbrek.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gngaihpwu.sHtML

C#:   u is User
来源：http://mobile.fanxiaobao.xyz/Article/details/gicmobdyp.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfthjytvq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffaelfzk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gmtjyryvf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gnislmgyo.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gwpzmivwt.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflejyxhq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrzkmiay.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoyszljk.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoeojmnz.sHtML

[G15] 枚举
来源：http://baike.fanxiaobao.xyz/Article/details/grhbiwseq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghczubpcs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gojztpksv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoypnpdx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftgoyphy.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/grreflirp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/gwlqlojbo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gsggqinji.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaglqgrvf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fanxiaobao.xyz/Article/details/grfftflxy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuytbrfv.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkadlepg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsimreb.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfvsyadz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/gllkimedf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcwvcsgr.sHtML

Ruby: obj.instance_variables
来源：http://3g.fanxiaobao.xyz/Article/details/gifvobcqj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gjiaxqjtw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdgmzxwl.sHtML

H. 异常与错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrhypusw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoylakhb.sHtML

[H01] try / catch 基础
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpktvecv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/griecimva.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcrjrbbd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fanxiaobao.xyz/Article/details/gzzgpxxit.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghfsoootw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhpbvore.sHtML


<!-- 参考信息 -->