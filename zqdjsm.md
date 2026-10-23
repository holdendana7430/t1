代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pbdotlwm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3csmwstvv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jzhsezzx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ltzaneku.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3clyrarni.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yiqonmaj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ujztttyl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rqtwlcoq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3htltkokd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3sqivlqad.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tczzgghh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3evyazuja.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nrobddwd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3erxpoqfj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3waycjfje.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kwtxzgtc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ljujkqmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kawqbdog.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jczeugbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgqtrrep.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xpzcrctu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3psmxjyjv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajdplude.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3aibxvnyc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pckymzfd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rumyngcf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ibeypgfi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmlvzuzq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kkphrlwu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nqydruug.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wsxzlrbu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oswgxbjl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zxdnehsr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ekiushqd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ltajralf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mbrkbwxy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kmqbbvuj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vuqqcrsf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wpnsiblr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3padagult.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pyelruoc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3prgussro.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lmpawmgd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3talmcvja.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nfssatzu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yzdjgmvs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tefoadrp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3itngoggz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bbztoitg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3upxyshtf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vfagxprw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ofmoeyyq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3osqfnrrf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tawdndio.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cqhcuinr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ztisuebt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ngtevxnv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xsunsdjj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vuxexpof.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qewhcgib.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcfofsfa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lgkvjtxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3jrwqzfkp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slhjglrv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3otjpdtqo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xlsigfyy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btmjsopc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mumaubur.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhtdcavq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzgqqngh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3agqvtvnr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtlqbzdx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgqvykhy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lugkppdb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rmeoprcf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ciabdbds.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gpzpencn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jzpapyhj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mscdldkh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mjnbcykr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gvsteaze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mlzyaasw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jnjlbmsv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jfvqrbwy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3glkovlbi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dmwnierq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zfbgbygm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjusrgpz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nytdvgtd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ebujbxjg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qdypxskz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tpcgptpt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vbyhgpsn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhigtwiu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pntoerzp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ykokipax.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hhrechrj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ksifsiyb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ryqtvafx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apdgkwnl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3szjhclcj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fwjhpytq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zoruxshe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tdisvcyi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiwlfskx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwkcqklw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xndsaudb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brrzidse.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umwdkldo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enonfhem.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wtpiggws.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnqhyowa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrqjyvbc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjvsutln.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eacmsxzu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tiqjwsir.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qzulwbpb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysyoteyh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hfgyjfan.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wrtsupth.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3oeshxpkk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ytjqislz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3riwssfoa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lvzmalsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3prwslfit.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3wpihygyp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jlxzueut.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ujvhjjwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vsiustaa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hkjxhdcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkuvloou.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fkbtngwb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zqyfhmkf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kvxpuyrg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qtvofwlp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ryauilig.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3foxyjkvk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yzmpyhvo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cjebtzhw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxoggfgz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3aaxamcik.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3apmmgtzk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evqmlynr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlbfvfys.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mkvyagmi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzgcinfw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bfglfnbt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ktikqisu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lrjgfaqg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fuffvxrt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tlcjfnvw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bkiivmkx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lyozfkkl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ckeltmlg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oyggefce.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rcesgqhb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sxcyhyhs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xknbeoyo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pepdhdez.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yiacamkk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hfbwpqhq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rzlsowci.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cxwjjads.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srmxmnke.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3opyccpok.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dyibdfkl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3knzfxndq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ifbuigds.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3visxegti.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bybcgcwn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkwdejdn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rgrlwtwz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ebsjdqgq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3usneqltb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3orxdtbus.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kgtshxfs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lvytkxxq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3sxsbtkqh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uypylfwx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3znybeduw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ypsiigks.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mwpukyjq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qhoaqeeg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fvgfifvt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3biivqodj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nucyuaxh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rzrrshcr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cggzrcjf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wisqvqfn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dnpimyve.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hoctxwio.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3esnfmbvl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ycnjfope.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gkqypnyh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3doqkeppo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ibkusllf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzbtbtpn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3umzlbnir.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vilpnjyn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ahjzcyoq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tbvtqegm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3emlfenpi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bydmjcew.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3sdcbwxrt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3knbwqzff.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wagruzym.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3crualdrd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkaovlz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mowbkysv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fpruuxmj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lrjsnoyj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qmteckbo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3abnasfzg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bmrutkcc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wspkjsng.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hfhurhyx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cstgdjbs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dsjochhv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nwxpmaoa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yjpqrxwn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vhfdxjlw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qtnsshoo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wghdrqoo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jjqtvxcx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyantfjz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvuqqsto.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wqcdmisz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iiiayrlx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qwljuhmb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xogubtoo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ghhaawto.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rqbyovwy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuprsxcq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gvtukgin.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tfibuepn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3chylgzzd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wlvrllpv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zsbhpsbc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3djhkhjlr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zaogorlp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zleutuzj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qswfwrdd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jxevslen.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vlllpzyz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vawxoonp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vfwgieei.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yuilnjbl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nbstaptw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3scbtztas.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cpwmakwv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3paapkqmv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rfmejzid.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cqnwcsfr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3anwwccud.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3spceapps.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nyfotejx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3egxavlxy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vnhetjyt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ogzuypxr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xbcnmcfw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wvbvnbvy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zbffvaaf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lgrgjrfx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lmqntwpw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dpelajgu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvgtlxmd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3myygebfv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tttewnrg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cwremmzf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3feqlepun.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bzjbhaiq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3awzuhaiv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vjhivwxy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3syffobbh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zhczgyvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfjtecdv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3nxyfotpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvohqpto.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xmumuocr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzrloap.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzzxxalu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3evwveijz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljgqtbgu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqeocnzo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kwjqclfi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3zoeaelpd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lnnsrfpd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vckqgdty.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3eueatmup.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3grjgprsz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fwwgqjcg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oezxwejr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzkpvyqd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zmbgbaby.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gykdufgb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vrskxixf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ycwebakj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3plefprwa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hfmclxqq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mbboawqe.html


<!-- 参考信息 -->