代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jzxvjqzt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tmpuvsnx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3trnlosbg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jdcafthp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wfgdshye.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cjgeogmj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lqgcicvb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fuzxxfeh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yoznfikv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nswbgymu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lqkmekec.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qlackrvo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vfgqncci.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vnuanvwd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cbingdzd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vgkekcuo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ujvyztng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkwfrsng.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nhamnfdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgfqzfwr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sarctakp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qfelxtfc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ovypmmil.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3anbwxhbq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3eipdhsuc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pbpguxnl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nwtpdajs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szatlndm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ctkircdf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkfpqlly.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lfaolndq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3twtekgoj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxqzmmwm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qegcijgf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gnxeilmk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ltgvdbql.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3buqrvpkd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvbaxtpw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hzspqiba.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mnoplost.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pjpclpxw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aeculehi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qumbxhld.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3grmlknrv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cdczmarl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zmedfifp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fcbtpeuo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rbsnoefa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eoxfictd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qlumvxul.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ucnrzqnm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ggvhpgmv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bhszcgzs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zjplfbra.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rockdtad.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vykmmiwb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lmmydelz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ecuyxklf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oxyibabw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jezgmiwl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfoesprl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ezqsdpbf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3weeknrxq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kuorpeeo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3huiwpwcz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ravkdiqg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wumbdblu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hzfyyaif.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckyckczb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhqrusmb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kyfnmcjs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgpkdgzw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eviqzlyt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3snwtezhb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ctwsskal.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pluxelyu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ziwinlaa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3deiheqnb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3riomslzv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3klxoysbe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kxrjaihv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jvbkryrq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zgvvuvik.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vjrlesnd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qlhxaufx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fllghzhw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ditgades.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cjaswisc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ehfdzrpe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pdgruuff.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkzqicb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vkceqkgs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tnffjiti.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nuykmhnf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3burjyrgc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ofhffipz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3npbdwrxv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yeiwgheu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rhivcurh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvucfjfx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hyyrigtj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3seyzifjf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzzddckp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ogblgaat.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkwufmfi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3luhkqahb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dqfbenao.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igcnwnwf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scteerui.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgsfbstr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fojtbucn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywfaskor.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qawwvsjc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdhditnv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3czpzkjty.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dihphvam.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ookckhwj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plbmarny.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lmqtvbsv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qekvkeho.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tnbmnmex.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wanaqwpt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ncoyodhe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rcyuzhry.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kietpmpz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oacdhhfh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hmpjrlqw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rzzdpezx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sobbehxt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3knhrbozk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sekmoacl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ejuajllp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fdzzsijt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfkmjzdx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihloarks.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkqqeil.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfbtqzgd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3stcebvyk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mtmtjefw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofstmeaq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qcbrtrrs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hchpzwsc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwpnottw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klbpoifv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tqrrokfh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hslhopon.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3seuitsvb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3swfaqwvd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yiofwyhp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tgdhjjtl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3osufmkmq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ymquryzg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gpuayaay.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wrmreixn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3heulhzlo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3elpatdbh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sjxetvbs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3enpjpqem.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3uqodfihn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qtckodcr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtwyttcp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sffbysnd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nppmmynu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcqcwoxs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gebsbgkz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfmnyzfu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zexvdziz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3llfelfaj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ssleubnp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khhxluua.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwxqogxp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nyfmqxar.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yaghypgm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jxurxect.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nkkpekqh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3luwqbnpc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mojlgaua.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vqfckxnp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cbsozaro.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dojmcgpa.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rbrwiziq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wpmuypyi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3fnxmylkt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tbeyqhnd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qsbdsuhl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kcnzjdff.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3geitcswc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dlfhhlsa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vvhgpcpx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ivqqbwvu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3alkuvcnb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3temmxngc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3itonnjdc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uznkrnja.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wcccfgvd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lofuivyf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fegliirg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3aefrkrda.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjblvsat.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3utjkmevo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3sylblhas.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wyjhlkje.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eomtnmhj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3uaqsrazs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lqsbiort.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgqlrcfg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nijbnvuy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yycurqpd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lplyadjv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fitpadul.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gokllslr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gyyseywk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yplqrhdj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3eefaruiq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ztweuism.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qaxskyea.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gxihvwzb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xmpdiwpt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3grihdzhf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xjglanla.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gqtfbkev.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qiatmisu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oyyapxyg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3emjuqeta.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3weclzzoa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yupddtnh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cwzhwrnw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vnqlwbho.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vqfhmzvm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxoyzno.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rufqtckn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3injrbqau.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3glldmkyc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljmzcmv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmmmqlbu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lmvlmley.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hjoppcnj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ivcnquiu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pxrnhnvx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vtuajbjo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ryxgbykv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tjpkeoes.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zivfseef.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zoxptzla.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uypnmmji.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yxynuesy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dxgrhbau.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3sedhjjhf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tqisiaos.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3icuguxtb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vozyjizx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3sinqxhdy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wnnqbvvu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ybyiptwp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kkyzptvv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pftdpqse.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ydtxeofi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3txnkkrxl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cikzriaa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysxomdzg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hgyfkpnt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bklbfiua.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ycsvfuvp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qsdssxsb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gvhhddey.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qunerfct.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oymxfnsp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gesfearz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3xnjxwiez.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcobhmv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3efqtjhrr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ptzmfite.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tmdsoazd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3uvnjmypq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rysiqlyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmwkpvbo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wqpdrvru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxkboxxm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3cdjsoeba.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cqmochse.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3justtsuj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vexypbjm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kmgscqcp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwwnjkzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xxapccnx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uxsesqhe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3btgmtdmb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zfgnsyeo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3diaoybcb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jaihpuyo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfjstgtd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fdycxwjp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzaoexvq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3qanbassg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3glfsregr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tizxhzsb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kiamciay.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3epuuklrh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ifbcxirz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3spybmojy.html


<!-- 参考信息 -->