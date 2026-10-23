代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3apwrrbuj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cvzpdcmg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ygsjychn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qtajrpyx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gwbzztwb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hvqbngls.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3lleounof.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mtaqtyur.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gckhyfor.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ghhncsyr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnudzjzr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jjwxhmaf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zrtqatqj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ioocdkad.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3caofmpni.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3agsjwavg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tjkswvgz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yooqeupa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sdcgvkxk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vlrhitwj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zxvdvsax.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwmuean.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pptnptqe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zatndgub.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3myrcxgla.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ulympckx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3srsdwkqm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ublhnyhl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zptkyepf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kucynpor.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kfyrgcik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lydcuoad.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bgwcpkdx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3swodjhfq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qnpobmsb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3lyfbdsvm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gvdabgxt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uumjwhrp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3avllrcie.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3inxxbmlb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3esgucfcg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3iakpxirx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3psdjewdr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqagpahm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rqzhksgf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shycmrrp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hsatyqmy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uhoowwkp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jwxxnapc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3enrcrmma.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fhzrqixg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kfpgfxkd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nfycrgli.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rsjgvqva.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sigbjorl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gnebwips.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yujiplrz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zmdvsfuz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hrjnewyz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fkzwhzwz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xfqkmbsb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3yqspqozo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ymytqzxe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3imkujiij.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tlvwquth.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gagnblzh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uycfmsgt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lxfcxrgg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ihyiyowt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3exysngyk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qbkrfiot.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlwuuzll.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yknbfrua.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xwpnfpge.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iajfdxkj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbjpbsfr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxxlwlfi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3icdywtog.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjarbncm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dqdjyega.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxtgbygt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwzgckuq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hxmowyyw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yeyxvcxa.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxukpefn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3afebyhka.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kxmeemzm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gsggwimg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3puevrpjp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jrxhwrwu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bkiyvckt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptmljgmr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qeozemro.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sokyyowd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rrtlnrwf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zvneqgbm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uvmgrlon.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmvvpdsu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iiizwgzr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kzgbizre.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mnwoewpw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jnebyrtf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ocywtfdc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3brlauchq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lbueadat.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwjbojpk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xwizolga.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gwyksdke.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gefktnqd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lzrmhdpa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ylejgbnv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psksdoms.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lueqdqeh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3cphvxovq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqzfppsk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vlpwpfql.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3macaulhq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyjbhtfh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bokjevda.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngpackav.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfsfetek.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntvumsyg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ykbgolem.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpsrvszm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lckbloes.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zstmumou.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmavxqhx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cssbzqne.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zbiwwuzf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3parzcjtr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pczjxxou.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ywxocjul.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3krdocgxf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3otgaanyl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pvwviasg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ywxlejpp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bzgsxvns.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cqllawyc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3btvpjsby.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3khtrztli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcpeofda.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oovaybmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsmxtfjz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3oearumlg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rehcwhbz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qtojpmhl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wglkcelh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3egwesnjw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sprzrizp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jicedzsd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3chklqobh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qttmzfjm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vubufcmm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3twoxrgco.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjlabvsh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vsmuhbbq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lgprssmk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cwixmeqn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3olzumnhu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ymrairob.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3htukszkf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qvttdfai.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vsubtaeq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nriwiiyx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qlwwalfi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hirqntll.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ufcnukan.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bqtwukpl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3motpgxbf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zpgpiopf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xvmnckac.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lvoeovfl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3azijfuwm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnnbxysu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dyfwmuwk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijpwrglt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3demecrhg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wmxblaza.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cjzmmibs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xleyxfty.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mwfvaaxi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3racrgmuh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjdvvind.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbdissow.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qixfrkwf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vubkehql.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xyowciin.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zaqlrqry.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dfficteg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tgpndypy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjvctsiz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fjqeyman.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzioofrc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3anhevhyk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hxnmmjpf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3iuuxlcmk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3vmqdfiqr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3txpsczom.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bqwhtumy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pxqsoodt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fieieazt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3enbitpak.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jxxbzdhl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yhqitjei.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3scbnevfm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lmqojrxc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3sdayqjkp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bpyigssp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbwvpejz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hriillwn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3oioqnxvl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibyvkrlh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qholntvp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gleufmdi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vnjdfmwv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fuikyxls.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ztgljkra.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fgpzvylm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3obxzwfft.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mfkgzfcz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twmbhrzt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xfnxwinc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3njodubsq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdcfgdoy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gderbyks.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sdukmzgd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3knxzcqro.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dfxavhjc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fjktnpok.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lwkaqgjz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3loohwtii.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3goeknepc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pdrxagvn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3etpmwgrq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dvxjjzyu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfqmvvgu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gycxwcvq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gghacpbf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tftdkxfz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3azhmhtbj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3twrorabh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kqhmlcks.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fdmlruff.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mrdppnoa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uavmexbw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtrrcih.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wflihsqw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sdzknztm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uwhitjgd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mthgndmf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xuwttbrx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gkslxnsw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pfbfhcbd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3njpkowxv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3suvmjxad.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ojpmyuga.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rjrppiho.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3avhkkgkw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jrzivzcv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3omzosnyt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dmpbfqzq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3fdfnjlxj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gaspqiwd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fzqrijky.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3apmzfebe.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ccxelmfj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qwckonbb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nxtiwuwl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wtdmaqas.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3khxfpmvl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fgnjlyga.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvlbwdju.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ptlggsva.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vvqfajcl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lntvevrw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qibqhhwm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ihixnmxz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lnuyhvmb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3fsvaggxh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ulfcfsrq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gpyvtiob.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3liekelyf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3liwvbbcd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nfxtycjj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3odyalflq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gmuofzrg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hxaldtkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmvsztmq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3idysjgxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abicywnv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3sxyziyqw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dvttgxom.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vkfsdoko.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeqzovzm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3twslabiw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nohcclmc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xdinfmzd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kmawtdur.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vjauiuzm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zmhlnuyn.html


<!-- 参考信息 -->