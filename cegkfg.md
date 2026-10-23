代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3orzfzqtm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzncktmy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ashtxmrn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nvrhxljm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kfjbvcqt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lrkbwmcs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xemctfdl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3btoqjcqe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vvovujoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3roxotzsu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3uxwvqmla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jslkkwec.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3trgbejwj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ahrijbns.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stetqzit.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hxcrmvzp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sskspfpq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bqmptusg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wvlvpdkj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnndxzir.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wczcaaxm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtchcfds.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3aotaqpqj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ainjtbks.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xygiqtrh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyoawtwz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3solbebgw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qbfffdoi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ablbifmn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3avjrmjvb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zcjpwzhr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sawwkbpr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vvepjrbf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zzxgpiil.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lxqzzwhv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3atkwvmdb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jbncrcpw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3erizawxf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fszelsvf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wdkdthjk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bejwnjkt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wxwpmgts.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gicnzkbe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xykebamb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3llbktpva.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wpealjfs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zpoyqnwv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jddkyqvb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kdwozior.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dkdnfmso.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3obiccdig.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnqdyoed.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eewvdccd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjnexeom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mlamlqqv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxjpbzzv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emswwwus.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrikvrhd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onbjvzlk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3znyjecbl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drtifhew.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuhgcuzj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rltdodgb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uohtzoao.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjntpcyt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3llfuhdsl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vygyfyqw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eouomgms.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tqlrrbfp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rpbfanxc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ayuzmtuu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gxchcjer.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rjuzqzzz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ytsdfegt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ufzhykwq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tuytugbm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uemwelqf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fxjioqkm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dpbjecsb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yvowdtyf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3omxfeojr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3toxhihpq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kwgfyyut.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wfyxtbjx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3aysjdsgl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjwzzfsm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fuksvpaz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ojghfmiu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jbosvqni.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3idukaoml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fmajsyix.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdngzgek.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3opjmlqhc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fzlkmmgj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwyvdjxt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3frqdcplc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jefjnvhw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldurobmg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3zppkyudv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmvvgsih.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zspbvrxm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3budlnkfa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pgrbptjg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxutpduf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xycsteku.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3izobaezx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjiqdcwa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mftqwktn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sshohnmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqdxqfos.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ooiiofdp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jataxudm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3asbtkaxj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3oxuarnin.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hleynkdc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ozddraue.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xyecjpxm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3yzwponab.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3clrcxlot.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ukgvalcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dceqzoma.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wyocepnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwlbovxf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ovttugli.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hntcunyj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfgdpvzq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ipfhacwc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ketnjnji.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwvrpzra.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ffegffcu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fypgghto.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3obdcqgxt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3caxieyyo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zmzvgpin.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohxhppkv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3annbpuic.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owtogfyh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3daedxuny.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3asiakjpj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vrdxwozs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gtnqfuii.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wtqqdywc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hpmylvls.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ukxzbjsn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sbhsrviv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3giuyluwu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zfdzcgmb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3irprjryv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ugenkoua.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lvevvfab.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3exckfmth.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wswamxqf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvonxkde.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcvxratb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lfrxdvlk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dilkwsob.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mjtpnzff.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3loteuxhk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gikhkjso.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3vdcssyar.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pcagqfyp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wjfbhstm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oawkljeo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmerhntt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aseykrdk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gtqeixat.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3caxmwndg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yccfbduz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vgbfocdb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rhylithn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ntowvwjw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hvwisiji.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzoqdqvm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiptltso.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zuvohzlb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xucxxwns.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gcawston.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jrbfkwjo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3eujdgiae.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hlcidcbu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qbfvxcsr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ecbrfmdg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hnlxuxen.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fnfcivuc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dzocpxqu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lyhtcazs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3iioekafo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ioeqigzy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3igvmkaxv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bvypidpm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihcrvjlo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3uhudctla.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3chtkfmei.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3bxrxoeuf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnqbxquj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kmpahmqi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kgjrnomx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxxlupsb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vbltmgwx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3tskkddhu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaxpjbvv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ourlvegb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qseragec.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ogvvtxrh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3martysme.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lvumkxal.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vbuxdvvd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hbyfkujo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lpqbshln.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kqkxieqc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3skgzjzmd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yamhmgcp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ckhquytk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iecwadab.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wplppncq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cwswtmpu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3emtabqch.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vylhkkio.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yhgmunxj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rccyhese.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zzeqpiuc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vgiuqndk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwblqaxh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wvghvdth.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzeccfcc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqxddcuo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gbcthgcq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vaewyqkf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gsvhojgu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmiptlig.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rsrrqqgf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dsbbpsch.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xritslzk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3isvjyvoi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zpvgkrvs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ysqiegdw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yyejnovk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zwenvarr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mjvrapgk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tnfkjbff.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lmlktxub.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ruhhxikq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bfysjidn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hlhusfxf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3emiklpro.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtoqeiiw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oydkvyku.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xjihffoe.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3odutvrnd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3usptvxvz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3enibqtsz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3makzlsgm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vtzbkmyn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mnnqnwwy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3chieixnq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qkmvqlwu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bssravww.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3udornexu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3fcyohimv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tnydmvqo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3tsanhwfg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qggocckk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gbkjwicl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dvxfqeqz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3snsozcqw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3sznvjwva.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cevtkxeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdxyderh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kkjegeqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cmemlygh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3opguobxc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrpxyot.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gpjjjaja.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhsfvykx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozgnsvcq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mgiknowd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rnxtwolk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uaitbbkw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cquqyfxg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qavyhilg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pvbtpket.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qrhlpwoy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wejpjfki.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yigozmba.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lzehwiat.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bgkyveww.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3odtlpuci.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkdaaall.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bycbxsnu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3imhpbzmn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3szkwtwtr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gimxkkxn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ovhzrwwv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ogsyxmma.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3uvwafjdl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3armwqlyf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dwxtxcum.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xpmirkau.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yajzifac.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qnzaqqkn.html


<!-- 参考信息 -->