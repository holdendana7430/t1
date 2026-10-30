代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/ggrvostnv.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gxxpjeydp.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gfttivrxu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gpqyrxvpu.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/ggfxsymdx.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gnfvihmmb.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gapsyueqy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/grqdgrbhl.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gjnfokcvh.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gzhdwjnto.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gaghthfgk.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gqlpnmibh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gwbtjriqg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/ggagxfdzn.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gcmebtkei.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gnlzuvcmt.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gnrcoprmi.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gnklibzqq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghcfqcmfs.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gewzpyfah.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gtncwxkch.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gaegtwacc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwmzxmjuj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjxrrrifk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/giofcvfbo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gjcohxcez.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gawhfdgjz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gqijewjwn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gpzzgmidb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcvxqxxlj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gzwqfqrnw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gixgyuoio.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmzqmkyps.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gsauojabv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gfuiwelro.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gkblkgwua.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/galeewowj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmqmfhlhx.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gxshjeqas.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkytojuyy.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gsjenvuas.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gzflaaupi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmzmouvxj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gkakzgkoo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gzszwmudz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gynuvtqvp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/geqyaovrx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghnnxgwzd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glozrggbp.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gofeuwcgx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gkkeiegvl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gnstglvpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gjkamqngw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gxjepwxmu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gsixssrkj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gtrecxgsu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gwgdmgkkr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gymompkud.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gaumnugua.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gdcprpjka.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gwjqlfkai.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gccthkqui.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gbsikesjh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gphperngu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/goihicjfw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gqzvzzbwg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gvifotqmu.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gyiuggwbx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gffwkjcxm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/ggrwnombe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdkardamz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyowkxkcz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gopbbobwf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gcpqwhaal.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gjmqpmobm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gpydmneby.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gkxxprbtz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gttutdnln.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gogksejsf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjkxdbrte.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/girrpbfbv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdhlizxbv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gaqzwgwyf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gulinipak.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwbocrvwd.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gltdsoxaj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbumgrkkz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glbughhbg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glucnfoak.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glpsuuhpa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gczuiokhu.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/galtaglqh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwyaveyus.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwgnxfrvy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gmpojxwqe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gtkvizrqg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gsufbpsss.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gjgsnedci.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gocpzicnr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gfsnbgaoo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gvhrvuzzg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gfxdgnpzg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gombbqqqx.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/guadbziql.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gnnabzhlv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbpuavnp.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggtzgssjy.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gaftvdpsl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gavzfmkbc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/giycblkzm.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gvkpkcgme.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/guapdigpv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gdlnwzuac.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpydfbteg.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjvyzhmcd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gxmhkbueg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gqvbcseqy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gmwzslelf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gzssawbls.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghtbmtktk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gbnobxroy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gfynixyoz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjsysctvh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gslgmfhup.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggatlayqs.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmrostnla.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gaqupmzni.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvsyukjsx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gokptgoxu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gezstbnlr.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/ghwsdgmbc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gisqjynig.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gigkimjps.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gxknqfctj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/ggwngddgw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gieadoyve.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gdepsddft.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxzzuyhme.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/giubagkbq.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/grlqitigb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gvyosjhok.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gyaouwvzy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/ggheamwfc.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gzxxuwyjc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gsmsqqbtq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/glsblhqgv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gehxyvcii.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gqpyjkxlu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggycsaxne.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/ggagswieo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcitothdy.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/goouzwtvs.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gffnhblxf.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gnhzxnfdx.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/grsilwlzp.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gtvtxzqkm.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gzvsvczfv.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gxliumxmi.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gbcoviuio.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gdceraara.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/ghgbwfpnh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gwhjnljns.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gahrhrrtz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ggfgzsdls.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/giuokwegz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcnkzyraz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gcfwwnxjq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gnojmjkux.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/glkxlooqd.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gjmqhflwf.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gqegfatwe.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gnykyqzcq.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkqphpgky.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gfkosqeut.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gxzailhco.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzsnupnry.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gujxjliyn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gfgemvmwe.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gcztlgupl.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gfnllakjn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gplsqctsp.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gssoaxysn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grxwvttme.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvlbgzooy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gzgzagjzt.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gctmvxgit.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/glqlyzrlp.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gbvyitrvb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gikhrxuss.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gplewlxoc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtyrfhond.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ggzvpatil.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gpxdirkob.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gimjbxjvs.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gyynnldcp.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gqozrvfnl.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gtzgavdcl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gzuhqlzak.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxozzljxk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/geupgqkpc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gfemcably.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/getdxtmee.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gvkhvdbng.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gqldnjlki.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/ghvtxgqkm.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gcoogkten.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gmwoqhnij.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gwwrnvoxu.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gabkogbjr.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gjrdphiho.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/goultkiet.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gvvfjwfks.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/grmnguexx.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gcwvvtbdd.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gtjedkibe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gztozznrq.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gswvbcwpz.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gqqffhuqt.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gjyobcrqe.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gvepjbqko.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gqooxukac.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gazoxavkv.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gffqdxslg.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gqlgabpls.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gudserbqd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjxkjswd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gzefewsqj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/grroavrty.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gdxtbznfg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gfdsebygd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gkspiqjjz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/grpsnfsmx.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gtkrzgiav.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gxxtsphet.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gmrgbrror.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gvsgrkfdd.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gzbtmtygf.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gxtvrpyxj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/glurrktes.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gcqpzrglb.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gqmnuaexd.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gampmdpeq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gnairkuxs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gtserijlf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzedrobwt.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gcljdgykh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gshziaedy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gqrxuyjxn.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gwznchscu.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gznxsnjip.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gqkdxmjee.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gkhygldif.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gpgshfbbz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grkvarmse.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gqjvlbear.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gspmnojmd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gwidgraif.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/ganmubqzs.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/ggxuvwrxk.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gjquduuws.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gseelhhnx.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gpczcwudx.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ggybcpewh.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gnrpkxmak.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gojxsletn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gvcfbkewd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gvgbrprgy.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/ghmmgsimy.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/grzethoyg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gvfnmjxkd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gwucuykvt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gcglyujqz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/glbynnpvg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/garxxcaha.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gafhkjwsf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gkgzgcbwb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gkftbrnop.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gqjqufzov.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gfddeznmq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkyfzezdu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gedookdfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gtumqxgzz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/grahovfyu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gyvwhmbzn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gmsulrdav.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gabheydjs.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gdnxpaqao.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/grczglzto.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gopggygys.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gocktkixk.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/giweezegu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gpkxdzcyb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gghnubjfz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gidgimvba.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gwgfbxcbl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghihajrnn.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gbayouslx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gourgzyvz.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/grbsfzsun.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gkvqdtxrm.sHtML


<!-- 参考信息 -->