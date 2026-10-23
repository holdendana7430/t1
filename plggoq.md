代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kpnnyqlw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iginxrtl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xtsdgaru.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgatqllq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qvznyxnz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3emavwhwa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gsfcufjp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dccvmapy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3bbcoashh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3svdtdjeg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3egxzwxxb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rmljxxad.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cnnkitha.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vfaqoffj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dndfahhm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3nqjaxezx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nwbkdrwr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rzlmqydm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3aionuxqv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3eqebwmtz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rjlexeut.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kjumkore.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bqppxxyf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3djdqvmdh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ecqlwsbz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zowyljcg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3finxriur.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dmvxvlza.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3apothvcl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mcunjxki.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3devewgqr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tobqntwp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxnukpva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xiymzpgi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3uduqpdjq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnozxlsx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pftbqxhd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3gdeokppa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3seebfdur.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vugryrjj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3msuyolsc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrqydpje.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3raocnlid.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgfpamnp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uedojmrj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lysugqwq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vrcrqtbr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jgbbbjhp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kdrzhlsf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mrfcglkc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pgelbxuh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fogbfoko.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rxvzumux.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gnsggsev.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qkbojkou.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tioxnhpb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qccceyad.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rsfhlojt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uozweves.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zhlhltku.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pkaarzkq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dwpimevd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nqpqejmz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xmslhmzj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cpswchxp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdqkdecu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tuwihiyw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ghxhsgwb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xohletom.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fvzyleas.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3eekvkoqm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkqpnfoz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jspzcdfj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3izfmlftn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgnnxrko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qipxeyla.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvlauucm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnoexmbm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kgmdvdxq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxqetwsy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3joqincaz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfrqxndy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cohwbmek.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cluiqqyn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlfunapv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hikrbnvc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuiczpwx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xscpuytb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3bojgpqtk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdlfrbyl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3selosanf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mxxzvsdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ynhixwau.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dpgclzkb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aznjcrgh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xgynokpx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mjgddrlj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ctjnjrnx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wiphater.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yvpmkatu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytjdflbn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dfpfoirc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqvzqtns.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yajchset.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wotvnixm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxzquafg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnjkgtqe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tinexgou.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zhwwrcxg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mebkuiyh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dptnpvit.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3welgybke.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztarrrts.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3blxdlull.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvcsmfho.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xvohqbte.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckckapyl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3otzzixzf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ltatmtei.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ehrjmfog.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jzokjbkt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qjwvoagu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mgvhdabp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3njobtkgl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ibhcjzmh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jgqafggy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lgopewhn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rtprjccb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uszwlnnu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ailgeknt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kormzzox.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bddpokag.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kecfascr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mktunjja.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qnzixotu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjosiqkn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yzcpedfj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tfwceozz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gbcfviog.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3eqcudnhx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wtuwvgpb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jiugxgjj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3opsondqo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3btitdawd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3icfkffxh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uubeoezj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpnborxx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlabfyco.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rmvqefbn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hdhrubnm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xuwfrwqp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3alonwmjr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3izcdytiq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3glksrlem.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bskslaih.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ozneobmw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tvnaurbx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3akauheay.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hxucmhqr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fqtzhgrj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bhethbdu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kiouktyb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ylejejrn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yrcanjti.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kvasjvec.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vhtkznsw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kwezxtza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mfhutywm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vethrhdk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3derbhrsz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ruarweuv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iygqsshf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3bnmvijrj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dtdksdkj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3reuzshbz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dlpcaraz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gshzrbaj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3drfmxrml.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wxwcvlmc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xzsztdux.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3efhjqsob.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3opapoqcx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3oepogbrn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lhbuodxl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tdippsmc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ievqoyzg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xhoirncm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ahmvnlti.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mcooazyv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3oamvxhcl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kbxjuzfx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mtgjrlag.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3szjsazmj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3drgtdmca.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3okuprmgs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qawhcato.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvoocckb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3efldilpt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3syewmlpg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3itfdskdm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3osteqsnd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pauqrnit.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pofdqyaf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ddrddetp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rqrcvjcy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfwqzvhc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xpaplnka.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xdtfvwoi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tabdoonc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ehzoizey.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3achlozgo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zycjtfjw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3pwrhnwoh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zqhzgifn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xavprhty.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3khixhelb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ssljvvea.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zkygreek.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kaahuuti.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ehffslbt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lrroebys.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yevtdlme.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xaxyxemg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wgdnqllc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ilzqqerc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttdmcqlh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qjrilctl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wovuveww.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3rxajyqqf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lpuqlhph.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hijaepnc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3clhcibvm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3tpgcnmwa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ulinwtog.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cbvafhbx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wkdkbons.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3eoiwqfrc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pqtqrxxy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mimsngfc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3atspybou.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dimvlxoh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3smklkpwg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bqxwrjin.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wrpptcjv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wjtbaecm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3erfcedau.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xkftkuki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywtnytwr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hnnczzsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idajilwb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qkgypxlb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3iejexjtr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3mksdyfqm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aqxhtmlc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tfnwvcqn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwixxvqr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dfqzpejm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3urfhwloe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cpaotpku.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3npaoblvg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pckqxuyf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yehodpzc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3blyynbkj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3faesucqy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwwihham.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lexgaxkk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3syjuwbpv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zgdhnmtc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bmpqrtmb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3uazufbsv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rkbrmkwd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vtkezgbs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3isdjsddr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sblzgxcf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gcnctpqm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3otnmykry.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qqjnpgue.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hbtxddry.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3cwgsermq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qalqqjld.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3crqelvck.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3aiclrmgu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xlccrjnd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iotabaam.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnpvipxb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lraxemkq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3igrmjqan.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kwtspqzu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3qwaubxuy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wgtnqtsp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wsqvydbc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3faslvijn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dubjxfyv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cbppcqwk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaitlocb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qqnbubdn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ngllmgcz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ioqugnug.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gzxjsaia.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wbnoomqn.html


<!-- 参考信息 -->