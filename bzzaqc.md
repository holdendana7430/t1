代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rzjhstig.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3mylrahvw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xkhwutro.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfsbdayn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cfajxers.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yyvcjvhp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xcuijvjh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3btbhopda.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3awykwivm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fatmekte.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3jlcqinss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmjocikw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rpusfbjc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3wqaedygy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ckznmyaj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dxjlsjaf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nodjwofd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3euxslraa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3taiwztql.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syfiuqsq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cofwtkkv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3irfoxvko.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3loztnsmd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nupglupp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxgydjme.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnwkicfu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ojvvzqut.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nrzygnfo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zsebpsso.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvttvslf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hrnkyzvm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bybtzzqs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rsfcspbm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eychboco.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yynpwefv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nkgwovwu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bccqtvzs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uwyrrurz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ngmglsqr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fyywzcfb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3avrrjsvu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ncxnxynh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xkisqpkj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zvtatohd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zhpjucrj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3psjgstgv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rnbhnwri.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vetoqpmh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rsvxeair.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3otfgical.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjugiflb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhludrke.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imqegibh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndqrwqxg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3anmeszaj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afrlbnai.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ithvtmyb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmpwacuu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flqfdccl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vhoswdoa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moigpgdb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3finxsqnv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ogiividm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfajhxjr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjzqwoey.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qpbunbza.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3juzgjdxa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ispycddq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kbvqmbhf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cvinqzix.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qmgvdjhp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wazpeira.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lwhjiykx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gimmjzcr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kbpvyaob.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ssjeuaiw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nrmvbdnc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xibtzkvs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3abupilpf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uniyvast.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxvvuua.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mpgryclp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pmfykxlb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3oggpgkzi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zfsntdax.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvsbsbno.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3afbffdpk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3duztuife.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ondajjua.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gymwzkbb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3nbbqfelk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soojkgng.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3swlhymhi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3owibzkvt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jaweyeav.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mffnysjg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gatgbmta.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irdghlng.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qifrjxmc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwtrkcua.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhhxzruf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3muhxbtuh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ghwhdwws.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztzjmctk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zxhupdep.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvmwwnye.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jimcllih.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hzqylowq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gcumbxix.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlyerwet.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wtxhqftf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xpoffbad.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jtikcmsj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lhsuyxmg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cwkrvdvv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bwbdfjqs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3oreqrxdw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jjszuvwj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gbpadgki.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vayfdsym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eynaufid.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ycznkyxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xijmpasl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zttcswzg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jbzwqwww.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xgfowtdo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nclopsfx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lcjutaot.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sosqlgqt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3kpbrubzc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqdcknzj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iazhwwwc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3whjhnwsl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yavwuyve.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqyovglm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sxhbwilx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kpcklber.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tfwamfyl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kkbyiruz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hfgoimfn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vraudnbv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3sezyprqk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dqyatskb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3covpesuf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wgattqeb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aiqncnry.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tjoejawo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gdsgrjkf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kkljezbs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mnhzqcum.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ouaaagxy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ggaomdyt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jhqvvhnb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xjefucna.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3auglexqx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gxuwbiiz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kssshxwf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3toyrcxiu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hnelbkhv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3izpfulln.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tzhntafo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssktzerm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlncbboz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozfdmhko.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypkhcwyh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fnrkdsvr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zvxcykmw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3npfmcdpw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jftjnjpx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nfererhx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gkgbioej.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tijneort.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmygqylm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3quckcezv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jphnxgre.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nfhohnds.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ekgelcsj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ulyqpxbu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cmrealvx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3emnqouil.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sfevhiwf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wteakljl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ybzsurno.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3axgfabmf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gslhqqea.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ssxmojpl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cduvkvjh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3oicdjxpb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayohunuf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3erzdnkwl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyrecbcl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mxydczzy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hdyxhqoj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zobqsjjf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kmxbmckp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hhyphcdw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qbafriks.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hemnmhsj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3oevpvhey.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrlxhhsx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xanlpney.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3udbmblpu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vfdmtjzv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoapugxp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vcdigdeb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nsystapl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gifkwftc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ndafwvru.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vkmjkwky.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nutbomad.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ifqoovmt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kvkixuri.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pedxnuvq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tgcniyly.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bfrekenn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xweqgtmf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfuzuzpr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sxyxbujq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utsccxlz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qetwrcol.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3uoxugqyn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuickbnc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3quhtamxx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ghrclggm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsuugxwz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hozdbqcj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyrfedsd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dnntbtya.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hfsmbkut.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcgffjkq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3apcgfsbq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sysspidv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qflohuja.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ebxyqnsa.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbezxjrx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rnxrnxla.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nbflwnqg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yypiuizj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gyqppqfe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3lhswrhle.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3snaicnse.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zlikzsas.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zweuvpot.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hmffwcnn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mbiobvpm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aiejqoik.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgckoin.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vuxjkajy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xwumusno.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tfertvbq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3eoaimnzy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3miyadoin.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kxiijaqn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3laoauyuc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fiqlllzr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wqrxtpli.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3enwjvwdx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gbcmemet.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hlqadcar.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3roagxgdu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pijsbmfy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cgxjnrgt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mlbzlmqk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cjjneiqb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rqimwefq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qgbcezne.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nnndqlii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxqmzcrh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dkduspyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czxxkfbx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xmpupuye.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hplclgtu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hofjeiyt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzxxiamw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzornvjw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcwslecg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3weifkbuu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3anudmgyw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3heofdjzl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qbupskir.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pwpfqjey.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdlbbasy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdppfpcf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dkraczcb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pnhqcjpd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pmpmkqcz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmpkbkbb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khjrbchx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ldvymxwz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gcjzdwhj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3akzpcodg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uraepxld.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nrfwcrnu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pighdtyl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3owbicrdb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wtitzmbv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jjgbqkak.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3jigtcdku.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ftikqehp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ityoyjap.html


<!-- 参考信息 -->