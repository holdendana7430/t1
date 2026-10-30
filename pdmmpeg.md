代发 wailian999

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gkilpgicn.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gvhybgsib.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gjbgmgqko.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/grqjpftzc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gntlypmrs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gdxpdswkw.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gfohljihs.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gexfjvjyh.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gekvdlyqq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gwrhnedfp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gqvmggmbn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gaseisbtb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gmgfupjfb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gpdzhhnxr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ggisgqvij.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmdfpjvow.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/giccmyssv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gaqfjtzsy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/grhzdwrtr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gavpwuijb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gzbsqvthh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gqrsxtqih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gykmxwwal.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gigundfzk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gbrcdwedu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gwysaqhzu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gzxhghpxv.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/giulcirow.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gknilbwit.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkryxrjvx.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gwdjaeehc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyduojbro.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gjidlwcwf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/guepwanak.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/geyllpwet.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/glxyenywh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gsevjhoji.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gfkpjsswz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gjkvlbiet.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkehggtxo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmewfoazs.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gdpanjlti.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gezghcbdn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gyxmaiexv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gwiusbibr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gyvavitqc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gzvzwkleu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gtijzzhsx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gdmrbnafh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gyignrgzi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gzsbnlsov.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gqfwomlly.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gkfbkeukx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gjlihrobz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gpribhmla.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gymvveyqm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gqwtucnmb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gzbgkford.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gihuwmhug.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gngvwupjm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gnxdczuvs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gihjbckmm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gmsxqnmto.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gvmrwpwle.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gykjzlxnd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/ggouqetpn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gbrwvpyiu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gkndzzlvu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gyrphacnq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gylyxvpml.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfrbariqb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfqodqype.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxwbvyvne.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/genyntoqs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gtziykhwj.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfouovksi.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmdxtnlaw.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gosigfvav.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gihvjqxio.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjaaeuigp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwybansju.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvcekaoop.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gxyyloifx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvnxxupuy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmvjfelrf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyavanunk.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gkbonppdw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gepehgcxh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gsnmektjh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gzrpstiuu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gbkbdgfzq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gqbyspbjj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gfvniaiyb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gjefqdqmj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gfuhmxguj.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gcncbfjms.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gzbdqvgtb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gkcvrfrwk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gadyuzhgs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gsdlcvkql.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gombpgxtl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gzmpsekxi.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gxakdfoee.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gzmkvqzjr.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gsebjfjaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmetymfee.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gyvovwamd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/giblmhhxx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gyuylfkha.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/glblzzlro.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gochcdxfe.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gedmuujac.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gfkliswkv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/glzzmomsa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glmwhyesv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/geqrkuege.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkmzposwb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqazznbcn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gqbpagcwk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjzwjnwyl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gbdbygzgb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gumuenrxy.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gaoqpjojc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gbieyhikv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gxajnkgmx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/goasbiydx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gauboolec.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gfmdgfvmw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gtadkumqy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gyofcgfro.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gaqctbpwc.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gkvxvaxtq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gqgduwcvd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gteopmbpa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gocqhvbxb.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gyjuvlnxl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gmnzrbfyp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gzkmavymj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/ghdmgcfbb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gaeuihgjc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjehvywao.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gmymjadok.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwjxayhcr.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gbpechvzu.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/ggokjwcbw.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/guvtsqpdy.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzhxavmky.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gahcupsov.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/ggxgmdmbo.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gsyvbrqzw.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gyixrqske.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gjkyftdtu.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/ghtxkssvz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/giaznufsk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/glvxvfylx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzlcoomdz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gobcahdrz.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gppmnsdnh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gwtpqbdik.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gipzyevkj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdmzkxubi.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gledbjjiq.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gbfjufzqt.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gbvhbhrep.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gshzobudz.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gqcphzccf.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gvnavxkjq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gonoxsxwh.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/guuhyooxq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwlhwlvwi.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gkjdzvzny.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gknccoeza.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gclrjhnyp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gseddwqhd.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ggtemtsax.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gvognqdqs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbaccdkvf.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gbpndvzgw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/grtsssfpv.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gnujthepr.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gpnlznlvv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdhkhxmmc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/govilosnl.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvtvbdjmb.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdqqyap.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/geinzqkir.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gbkabtfai.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/guaeklijj.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gqpqizudb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gtgxmuzek.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtcgkktyd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbmciizad.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwiryelwk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gwhvszekn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gafppholg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxmzbaugv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gobenorjs.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gmbdumyjz.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gqthraufg.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gdpwemfxj.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gnfyobqlm.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gfbubrhac.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gdwfthswd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gvmzihmff.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gejtgmqlh.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gkhocdacd.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gvirxchmk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gegcwujkq.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnfcxghey.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gdmxbzhkq.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gsynmjnzb.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gqifdszav.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gncpgpqeq.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gpbfbflnj.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/goanaxswm.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gdwauwggy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/glyicyzxg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gqlqzufha.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/geqhuqmms.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gopgrjehj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gbxmqfano.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gwchgdahw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gfhnnupom.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/goouvkkgv.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gtfqhzkph.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gyirhmvhh.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gehxgjkdt.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gufnjnxfn.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gzetsjudv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/glwrqkfzi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gtpwpcuaq.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/glejoetxm.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gdnheyylm.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gdaansgez.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gduxzqtcf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/giqmfzyki.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gjyeqlqmp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gjxxnxtjy.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggtplwtze.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/guxffawbf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gcfulzbwg.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gwsivqapw.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gprhvsgla.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gxeegbzay.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvdsfbaaj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfullhnba.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gmzghukww.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvpntbrqz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gvgtkggtk.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gofqbmafj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ghzilxptt.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gvxqkacfi.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gxxeteaak.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzyknhyyb.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghcalrxxb.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/geciiwjfw.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gfsownzdy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gsehjshxl.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gghusddtk.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gyukorced.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gqcynywib.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gvsmvtpns.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gddsevacx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gtysoipvk.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gkzwnvduo.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/glxtwhymf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gniqlwncz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gfgqiinsg.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gjforhdnv.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gjfipeiih.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gjthkqgpc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gapuqdtvq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gisgdzpbe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gletmawcg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gxdzepklb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsxibjys.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/ghrivtlli.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gjhkdpbgl.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gzgmuiwiv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/ggwllanps.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gldbkfbhq.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gxrsrfmdh.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gtiotphsx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gsktjxewk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/ggralbskr.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gcgrpfdiu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gsocmyfrg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjwbqeqji.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gwhkqmltg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqkrsajyd.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/ghoiaivby.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gyosmelvd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gnzvqaqsk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gphniifrv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/glwxcgicy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/ghyomhycl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gutpmseav.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtzdosn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/ghkeyanfv.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gwbrxdksg.sHtML


<!-- 参考信息 -->