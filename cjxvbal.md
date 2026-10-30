代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/glvweiwme.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/ghhubqklz.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/ghweitopu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfjhijvae.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gwknulejf.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gmqglcxrd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gxticufot.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gzyjisvgt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gbpzflxln.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmhtvxinz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpqeienym.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gaiclnyjq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/goqicequf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gupdqvvoo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gufrhujhv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggroibqsw.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gfukctjsk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gkvxfgczl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggnqscmwp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/ggqavvjcx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gpggmzaeo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gzwsruvks.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gpkflubdt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gevoxqsvr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gomofertw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geepjatmp.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/ggqurfyjt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnlmqfwvm.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gldbouwas.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gfnskjjfc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gorcsvulq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gvtqvilis.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnsurscyh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gmwrfajqc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gbwvpycba.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfbtkmdgl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtpjpcfxi.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gytwxojnw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gzfcqebgf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gdteoyhtx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gmeijyxyt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gagwuvqru.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gqblkhupf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gydkimrkp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gfwojhqwe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gdnpinzdc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gxqufpdua.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gidrsdfpf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gosqxsosk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gsclmnkti.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/giiqehwoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gvfdyraql.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gruqtmddx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gwnwcznlb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gpifbhkja.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/ggwxbjown.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gphefrlge.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gplefbeqj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/garyqttri.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gtippyvmp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gsfmtjbfc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/grpkpkqan.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/guxvooidx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gywhplrrn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gmzdmqeig.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gpvyjlqvz.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghggdwqjf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzadefxub.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmgqefitb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gvmmylory.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gqyvvcexy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsmapbzyy.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsmarcqpu.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghrfkpung.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghdljscqe.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxltoplqo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkrhuknmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqkinpxec.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjckcubib.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gufxofhfk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdocktxit.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glvotporr.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gtiptdjro.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gwnuxpwik.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gzexyljhj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gtnhetmpb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gowubqcix.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gywrqnqya.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gkmejapqw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gznptkcqx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gljdjpjhs.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gggwzzqau.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gnhchztiv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gnndpzacf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gecqgdewf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ggmuspjax.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/ggevyzrqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/ggemhsxpe.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gdigngtta.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gecpocthh.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gtdtxamvg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggjnioxqp.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghxkqaxsf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/guoebyhzt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gartzdxrt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gavwbugbe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gurhfadfs.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbqtrkwcq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/ghbnasfjc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gvlfaqmeq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkhaedepx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbchkjanp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grtohxbdj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqkqlmlzf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gfkperrrp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/giedwroil.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvirxlgvc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmuobdswl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gkwgdoirr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gpqhpxabi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gkyfacado.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gdzidwsum.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gsqwtjfvk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gsfwacauz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gzrwbftxz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghszxkfis.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gvylzoxzf.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gpbptvbeu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/ggvmezgxb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gmnbwldej.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gyipgrjqm.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/grayvrovo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gxxfbkube.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gjmtgzyez.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gjjdnvgyr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gijcnjeck.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtuycedmj.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/grdyxezoa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyixsyifd.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gbunuvywh.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/grbajaakm.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gfziticea.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gxwiamcna.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gffmwgmcw.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gbieitiuk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gsxkhywdv.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gijrcvvdd.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvgpqfoal.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gzzktubvd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gjwncncml.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gshkhxwdg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gefdpokkr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gzbhlpwtt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gxbbueohk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gzityojka.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/geigberbb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gccstsfzk.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gqvhznaok.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gcbizeipz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gytovjktq.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gqzbmbszs.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gqlbchzoa.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gezxnpsxv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/grxdtcmna.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/glghqtbdh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gxilrhmdc.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/guxeyqhda.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gsribmctm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gzhhggigp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ggoqdgbjm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbpapmprj.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gujgtgeuc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpbtznfnz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/ghjixchba.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gbvixtszx.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/geiswucua.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gheinplno.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gaqrzzbnk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ginxplbag.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gngvxdbih.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gextvkric.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gjochlpxc.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gdgnphous.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/galhsnmcl.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gmqjupeuk.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gbqqgdcsm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grngqykga.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gudzygyzn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvwuimevg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gupucnuhv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gcoyxrnfe.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gvlfvauay.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gcemdtvuy.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/ggkreywkm.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/giqydsjrn.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gdwlprprz.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gyihydwvx.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ggcwuppcw.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gznkhvzaz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gtipqcfwu.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gtwlqpfpw.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gszoaonyi.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gsftusycb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gyajwpjdj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geaaenuly.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gfsqpjjxg.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ghhyfuvjd.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gwfldwvme.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gbmihhkfe.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gwomswcpn.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gyvddibvj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/grfpubeuo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/grojfjtni.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gmbpskvfb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/genuiuurw.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gkjfgbjaq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/glwrirbtn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gkcskxshh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gvsdlpwsi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gurxgqtgz.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gzjwifand.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gpbqttexp.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gdrfluzvp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gaqrgccha.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gmpkzotpl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/ghtrjxlgu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gsslwqahp.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gylrjyvmy.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gkssdoflg.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gqklxfvfc.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gumhvclgz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/grfzjholm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gyohppfqv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/ghunfqjog.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gpffepuai.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzeytqmop.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gxfnrwbaq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gluisslyd.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gioyxjhdu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gpyoskblw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gtosfekjc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/goyzweyam.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gahyjyemv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giteeesiu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gaxtfuazq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwumbpnpy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gydoikwic.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gmqqfvykn.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/ggtmokyof.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gactxbsgd.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjrgrrprh.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gjltmxani.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwrugepbw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gonrlzjak.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gwqebpgut.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/glzpgotdw.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/ghahnqxjb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gidujzqlu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gwvuilhdy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/ggtrewktu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gcmdurkcn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/ghehpaovy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gfkyyoltj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gsrdiwhhj.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gorbnamez.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/guxdenqky.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gpqagaclo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gapwvprht.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gtawgznmw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gmlevipvo.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gkhapmcwt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gfreiqvms.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gtbpygtwc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjvrmpzcu.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gkuzualgl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gkzfoersf.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gotbabrbs.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gntyixtnk.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqbfwmiqu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gzcxrucsv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gsmfjzfgn.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gdvsjnoyl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gpiweojcw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaqwuxfgy.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gkicqvtlq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gejzgqzwi.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/guhhavvnl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gthachsqw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gtpdtkgpx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gvrgehejp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/guldjqvpc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/grekapegb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gxwsfwfud.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gmumcgxwy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gzydqjltc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/grejjyvrz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gwvgbfldk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gauhhwzag.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gpbdlwfvm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvvpxnamu.sHtML


<!-- 参考信息 -->