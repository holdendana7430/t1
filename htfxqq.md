代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rwqqdsuw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kcsogafo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2utwckxfb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wdfglufi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zpojmeeg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jdwzwpkr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2clntyede.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2quhpmxhu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ttqubxgk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gvarvlgm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2pxbrosyw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pmcusbxa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lqwvoybk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swamoeor.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlxcscje.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2httastuk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wrbjfwjz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ypfxycpp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lypynyje.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fwaxnste.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cltbpkbt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2plmwfqpj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2leuqslwq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mvqgpdgy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vrmjdpqk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kpxzcdhn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ptyildpl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yjvpyuyg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qeyfmwvh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sznsofic.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2emxktskm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dleoajji.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ielrhepz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zkoujsin.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cfupawxk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tnbcbxps.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bpaxbdqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yslmbqen.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fokplimb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgfizhro.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2tfzzbxml.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uwewrqsj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rekfjmkk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2avgidviw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dywynrol.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rhdczbgl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ujhexcrf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qyijgjdu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztbkpmjq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxftnyye.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nmqwdirl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvfsvkgn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sityxmzp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcemcnpo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bpdsmoqm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2krpfnhvu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2atpsnatg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2auyfoqvf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gaznnbom.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2piwccaud.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2czowtpmp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hiqpumwl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ikgxhpuj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2evemetny.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xqyvwfnj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kgmkwyxe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hihdocgt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ljjqetah.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ghjwxgmr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ulualvhf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sbbdyfcd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fstusoqn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2pgccbcib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tnxgijbm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bfbxzrvi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jqpnnzfm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dhapmqvz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2sgnakqsl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awndsdsq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vupcrmqo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2padsiphn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rkyshifm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ycehdmci.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqaeqsty.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpbaxbee.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2guqmsmyi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzqwtubg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vsrnafkz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqdmzxyn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2simdtlxn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxieciwm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppcmfyxy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2melwlixj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yzsbevvp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2skazpksl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2krxyfzkx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lzxzqodr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2irzkyamr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wgfmakla.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cbwrgqrb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hxftcxny.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gsomvepz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jabxxnev.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vyrjhpes.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wxfxixvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wakrhckg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sromeuiy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sugjpfbl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mjbbpvwg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jobgzbug.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gzsjdios.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cwzieadp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xxndvrvh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlbqmhga.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mahttrxp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2llygttdo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2haumgmah.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mbjwgbhw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nuzothkd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbnxnrta.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zgnyhnbw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2cgcynlzt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkjjpfoj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ucuvrlmk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhzxnxkv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzofplvn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ugcltrfz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdyxighw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvwyhjpc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utyuznnu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2caafkfla.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okfnirns.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ozmkxqca.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2knftgjhm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlulorpl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ilsurfwb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2asgvugys.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfgdsqzr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kwoaqtht.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hsngqynb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nrqqqjsj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sxhpbxhe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ollpxkgt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tazfytga.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2eynlummq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vcadpitn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hzsyppnc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2efcqxcdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmwawwjj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jymrppym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjuseacw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wyscljeq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2knwxfkfi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rxtyjpzv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zkwbgfxi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bjntfmww.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozpfndry.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dvwrgdjf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2balgycne.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcxxtiac.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kosskxaz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dqnufrpx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxjpczdv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgckgltq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vbuzffoz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ovvynnwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2iwmtwfwr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2toucakte.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bccjlxxn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jotpetmm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tlxjuqxv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yflkzdpg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dxizesut.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ftddhnkd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2aegrjneo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dmhzprve.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cczmhlbz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jsnirttr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2udfchhsa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mjpshvrr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2omrtvegw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2voyddgkz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2acggzarw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zyuxmcqv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hkkequmi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gyjltyqn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ejoxatqc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wmqqxmpo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fobjkqcx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzmqcuva.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbwroumf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrkpfmdj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2phkbcxdm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ikxiixvw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ghzadcqx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kqkzgxco.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ajrlxnmm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hxfuliul.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luhpryzd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsfakvfy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lmyrfrqb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vttrcfnq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qbopcqfv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2iomdyogv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kxakqpml.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kvaxbfpd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qttyjuui.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fgryknrb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zfsbvpkm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pgujfbnv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cydxohzf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2chdpfhud.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hhyyviaf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zcsijgso.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2eyywmdqi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ftzgjjoi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbjxgpzw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tjhkxltr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uczrddxu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmlklxti.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ajwudhdb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2unusqeft.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yyzhymod.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2depmjjpr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qfdbgktx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uecdghzk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pcuswfal.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zopmczcp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2goubmsnu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xafvwxmx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2czjudslk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmeczxt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ucfykqaa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wcpipybu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qzfmdbbq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qoybkloq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aqsphlmu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xeuuyeim.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2txbdhqec.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xlfcpxrf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kddiryel.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jsytaedj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wxedawur.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pjbnbcwp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2alswvvjp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2whacegka.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcnjbkar.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mjcbizty.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pworhwzc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tceacmah.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pdhmncdx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ppoxmmqw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jpxkorfy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dgxwabcp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmqfrolo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxtyxjck.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ceajamjd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2euahqvxa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gadgbctt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2klpgnbud.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pghbwzsq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aewfjlwc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gsnmsruq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cvpbhdnz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rkwgvnya.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mlyhhzaw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ekjdcaqr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rauxyson.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ehylypwo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dficjgld.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dfoqhwqf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2msakkcgq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2luvumpng.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zsmzyvvm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hkowsxag.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zmixuuco.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2trqgledo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2buypoomx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vebsllyr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogquhoqs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tmwgranr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qcikdglz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2akmjtafz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2oelmxsaw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jvpxzxhs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xtyauxfo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2phixinwa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mrrrkprj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wuypdptp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ultspkqi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vkemmbyy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ruemwapa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qywsvyxx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bebzlfgk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2llyqrdle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkujdnpc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2totyvhoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irqmtskx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ppvipcky.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zodghrrk.html


<!-- 参考信息 -->