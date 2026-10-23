代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3trrnyyat.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zsrtvfyv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tebvmcyc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hvlhtybs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxeglgvb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ipltuqbv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gekjpxef.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3wjvlbsor.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ddqoaxck.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sokuzens.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aaarodaq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vgrmqyvh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3csczunug.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3khwqlljt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vfgirvgw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fvxojwia.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gqyqumqg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppknuxpo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3abpyhila.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yqqerzmg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mhyhvbzu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kjjobgyh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kmjwhlzt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xugyqida.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3imwuupba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvdbiwfc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3arvcktwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrktgwjk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nbcvgzao.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uzbyaeih.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dqietvya.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wyfithgn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bvvtwthh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mypkkadp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3eryomwcj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xanqfwnq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cmsnyzzy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hfmztdbh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lnguzkqq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgwunap.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nywecidw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvlvcvwi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jsnvsjis.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uzwcsgnj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vszwlewj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lceljnml.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3owvqlfub.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3luimyaxp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kuilnoze.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3buvmtijh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ysaxbwwg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fhwjpawm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fnhujrqd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ljwpcqpv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xkgtldcj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybxvibeg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rrigvzfn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3beyvzkdo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mlthiknd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eoqvldls.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3utwickgg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xncgaagt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zlgxtuar.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qcxplice.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hzecsagv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zktjueen.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xbhnaxyz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3loooxcgp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlowzins.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pswjbclg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3utrvaqwa.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzivoqzh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyvzktkb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3iqbyscvt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxkuktgt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kbcriafm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hiqriemc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwogeswm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3whpnexga.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3msjqowvq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oksnkjof.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vlcoyrdv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3erdphffz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vxamiwsc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bcmazkdo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3imivvwbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3veiaayyh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gpbulhtk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hkntdvke.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3iwrbfuzf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3aoadsyls.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nojufoqs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3oydnilhy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3daodxiku.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fagpsgqz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hwuurwbz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xkgzewvw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3abjfzoki.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qstalvih.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3phvjegmh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ffvdvliw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zudqougq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cbedctqo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lunqruka.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3agqrurmn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ghqfelnx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eeuawjip.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpicqqvh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3pldoqewl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yctickzw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtthnfyw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xclswtfl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiijvgra.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehlcbocu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yorptscs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imifhygh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqsahiwa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btlywvtu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3uhbvimci.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etekmymh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rlgqwaos.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqfonvpz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbgrgyxn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hihwrsas.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xrvzczrc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzbpdpsq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hpkfgsrm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wmyjerue.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3etkoogkg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3iybsxppy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wqxkybnq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wvxifszg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3shfvuxnh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3wdvuxzrn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gopoavgb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3obptjzfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwwtpbnl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3swenjgzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajdhudkt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3iinuorfi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fewginsj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcrkghvc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jevmnwss.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hrybnkbj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlnjcden.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ttbgcdzx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ksoitdxm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfgqigco.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xvohzevy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qkjiomis.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fvarvhiw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qcjpfvnz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgnzwmdn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hntqwnli.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pdtaojeb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lcnvupaq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bnynneiy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mpgnrdbm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3egqszawk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bgtpiqyd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eyrcvekw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jexnkzsx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3skdoybwm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kchzkqrj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oaxwhvrb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bdzdvvlp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kwqvkiay.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gkdigznz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xjvpeorn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcyktyzb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vrparhah.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vtjagyzf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ovqvxlpf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3igxozpvx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jjvdeill.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yviyisui.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mznzpxrr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hnabfbcj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3llppzhqn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jpedjyvv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zofhxazg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zmwpcxha.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pdzsnkzk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3esduccpk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ppxiduei.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nqbixcgj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhtzmjcn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lumlokax.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nelmvemy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ccorzupy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kzjjalmo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3fyipirmq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ofgbpryx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vpggfrln.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kztqcsul.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cnzvvngj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cugdlewt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bbfkissk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3itdebvms.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3dsqaawrl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bxbzoswl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3orzqvttj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3lxexcwxh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tgjalfna.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ahfksfxm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3azgfcyrv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kxfbmzdu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qflgmphg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nmpeykzq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3runbebds.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3trzymvyb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3plzbwypx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wgxdsgoq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxadlutj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fjtsaksd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pehxfbfb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdnwvzll.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pxhwaxya.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxxcanlt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dpngzrkz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ensqsozz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rvyznjrv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vwxeaetv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nvojsfyw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hvdpltfz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lvqulzei.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bcfkmzlk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fvmhwiez.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fkzpgorj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3efytckyv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ndffimyd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bvsmlcep.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hawrzlsw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysnxjylf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opekoaeg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mzmjexjg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3smakujtw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzskhau.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nszlcfzr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hzasocpo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jnhixeuo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejleuyai.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fikixzxr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3orvfryah.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fbmsgqzi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgjslgiv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3effivbxt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3prhoqrzs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jnmzcirn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wbajxvgs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ojgncupx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zfnvfojk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3soovrwjg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3laeumgtb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3joneqhtg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xwpofvdc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3zudzovfa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xhijuqju.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kclswnjb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xpuzumnj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xdszeugn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mupwayak.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ycbqjnye.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ammeuswv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3npuabjpx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zrotyafj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nystlnjl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ulqryocq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bfvwieuk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3trndblik.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rwlleijc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3krynbcwp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lbfijgtp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hodkkrze.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3adekleqc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dttnsqis.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3audedihb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3czdvhppn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qfwsurca.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3odmkyapx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yxkzudjs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3asbalavi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nagclkti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ymnklaqy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qormsjkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qeugzrpn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nehpgtww.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tctdzxvz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymzhvqyr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dkmjvzbf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aksdgqjc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mareskvb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ylznpioc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lhcujlhd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vclxmxrb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wizvhooh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xqltjfjg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dmgbroea.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlnmcgeo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhkmznqi.html


<!-- 参考信息 -->