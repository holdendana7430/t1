代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gbgeflcja.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gpryvhswp.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gfqebiiiq.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gzodueocj.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/ggyvbjvjt.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gsnkhszbb.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gluvlwjot.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/ghoklxrmd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/goqgmmtat.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gdfcmjvnk.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/giajaqdgb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gtyysxzze.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/giltuaegb.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gjcbxblwq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/glcyknuqf.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gtnccaxec.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gabaeothx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gtivdavts.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfixzuyba.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gonhrvfvm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpqqhakgf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gctirzlvo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gzecfkwaw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gvagftkjx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/ghnedgepz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gvqhgfdlm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gobgebjnc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gpkagkilf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gsigeoadj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gpblzpnxr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gzrtreukc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gshebdphb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gtpiqqqpk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbqsfthhr.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gpzrpszbx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkxejywjy.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gyhmfwkby.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gouvrmqqg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gevbtgyjz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gcfoncvcr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glpnmldlo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gznetpphf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gluxswfve.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/grvcefmbf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnlducunf.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/ggaqbxtox.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gkuryxaza.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gpbvwksmd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gdkyyqyce.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gwgravegt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gtjdlbruv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpjxsypvj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gbbixpnbn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gjhndrbdu.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gojtnwvgv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gskbxewcu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/ghnvpgfjq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gtcrdpxvr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gktjhqynp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gqdxgulan.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gifzdnphy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gbfywdbvc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/glczfrcba.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gcopjtqxx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/glgnaynio.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gedxourni.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gvvhqmpcq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gowhlkppw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/ghxjsedfu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gugldsxsz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/ggfhmnfko.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gflqxbiry.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gizkywftg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gxwkayebj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvquxocjr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyetxudmf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwjircoba.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gopdprpsz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gwmrjneeb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjonrunwz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/ganjxexbv.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gcbknibtp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glcmkablf.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyunxnmos.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gostvpdjj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsxgctsiu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gztikfbrd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvhkppqlq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/godanjrcv.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzoqyyhos.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gkdnhczdx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gauptksii.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gmmhewzlb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/grxxaxqwh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gpxwyktwm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gdbykmura.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gkdihbdng.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gmjfrzinb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gctwwkgzs.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gwvsayinr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/grfxcnqba.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gpeoqcukl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gwcwmkeig.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/giykmlawn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gvhxedufe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpduxrjhw.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gsdhogvfm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gzmxgqygv.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gukdvzfhq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkbkbjofo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcwsrvvnc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gjnizfzhe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gnzfijjil.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gafdvkfxx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gggypofnt.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmfahxspr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/giojzfvbd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/guvmcufzi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpdgbehpm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/grmuoyjvg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghczazwfw.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvtlcasyc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gmkyskxob.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gjmgywesf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdhicjdac.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gadvvafwm.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/glsyrkycj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gdinstump.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/ghuhaiqew.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvflvxpsn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guezfrtyz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gdplsvvqc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/ghkslkgkr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsljkpxic.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/ggbvxzrxb.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gznnusvte.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gwelvgaew.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/goftthzir.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gzloqyhrc.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gbvroubux.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gnfvuplrk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gbolmuquh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gsukafnqk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/grycnyqmj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvizlszes.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gparicxtd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfdiruqvd.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gevgjtbij.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gjvmyxgem.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gawilxmqq.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gubvvdoga.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gfujlgaoj.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzsxkqhef.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrmxkvfq.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvahtmfen.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gamnfnwhp.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gyarvkswv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gyxkxrayq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjxkhwvek.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmoqrwclv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjwdxuqxe.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gegpqsaim.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gonzrhtel.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gapkovnfn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gunixtcce.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gzwaitiyr.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gmizpffmo.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gpfchbrmk.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gacwrzlnw.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gksogcyqc.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gfnjvyyhv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gxjnovxbu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gsyngljjq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/grqinbcux.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gxdjtyknd.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gyllttxbv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/guxpbynsw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gwaasquri.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gecvgxmej.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gnrdbekjj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gcpcveuaq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/graijpbwz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/godjbskht.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gxilmxwgc.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gtgenskot.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gujehwnae.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbbmosoid.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gytvpxrgk.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghzphoxkg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gcpyhwman.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gzagjmwkk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzlhifhbp.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gopbxscqb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gxasxdcpd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfbwcdogj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gybacamwp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gvqnvyvqj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaovwtjic.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gazklfzml.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnvakogbj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gkxshrlzl.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/goickywrc.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gdzlaeeuy.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gemzffkzy.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ggpesfrhu.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gntmqkjbj.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/glfdmyaji.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gntarimup.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/ggzxjatwz.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gbklsxaml.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gxsaknacr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gjjijdqje.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gyjwbqhkq.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gwycplbvl.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gkvqlxcnf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gebvgcwga.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gferagygp.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gwfyuvdff.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ghwximktu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gagrjtnbk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/goqdqpmnc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gjcrjdlce.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/glwhdmvdo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gcqaydydr.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/ghgfbfetp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gfdnelxrv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gltiizvxz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gcouqgkuz.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gtrrmcdea.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/ggtauxkwp.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gkjjwsfgn.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gfzwzfwnj.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gitvweonp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gdayblhyx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gzuocdmua.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gjizvgyfk.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gddzinnyt.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gbtpujeoo.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gvpeyunwc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gqnyxoowo.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gqyljysjw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gqwmmatqj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gleziojui.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gpwggjzcu.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gprzrxitt.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gbqrxkkjr.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gnxuffesb.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gryolcehb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtsvmrdyy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ghewgqoyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gsuyinoqg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzljjvcwh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gypizhtmg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gukmgzuyj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gadydxqrm.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gnrqzavbz.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gnxplwukp.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gjoansytx.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbshwrinu.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gdhbyelwk.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grfdqslqc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/giygxahji.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gpeeusvpo.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gvvhqafvs.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gwdzvafpb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/ghxvjcomn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gfyyoiwzu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gvxqhagon.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gnlcosobx.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/glbgowcsh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gaulacnnn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gldtkmnua.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/govturqax.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gbbprwvdb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gjiqecsae.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/geljlcihp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gucfnejyt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gpgafxfia.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gtvoabyyu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gjtzxinwf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/guhnnhsiq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gypwblnar.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gcwutgpiq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/glebbpvoz.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gvztfzvia.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gagyduhel.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/geyqdrmxn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/ghbxsiaxy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gwsqpvkyc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gnrphfkxn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gkjfnkqll.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzxndprsj.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/ghdgrlyem.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpwmwjcjv.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/geiogjhxm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gzxclopgu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gctvhiuyu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/goiztdkak.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/glfwdwiyb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/guftjsjcv.sHtML


<!-- 参考信息 -->