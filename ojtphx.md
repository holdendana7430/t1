代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bdxpzohb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukggpgtg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bgmurrzc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wsstlkdv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nifwghjx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2chnpckum.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wfohfwwd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lffhzsaf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wusdjxln.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ceyhhmzv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qyxccwzr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gbqywkaw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2epabwvpi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uznreehl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nazsajyz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2axyabfqa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yalevyvw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xpraoahs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ttlhnhfj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ozjfmfdx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qoegfcxp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oyisvuxr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2icniaqcp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hlgejyra.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tzupdevv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ssfzsfay.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2thadgnra.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkmrdlyy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iektxlja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vikxwknp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2upjeeqyc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofgolxyq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpatczkb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qlthnsmw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhbgewrb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhqankak.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2almaiepw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sohancvn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xnjzzaha.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tepvthrl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvxahyqk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2efxrrbgu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2judelibv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lvchiybs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hysammls.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yvddmvvv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qhtezgdt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2cdqrwtmt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rgdahznt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2utjppvkk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pkxnhfyn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zulwzhtf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zjcoegro.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wovhzjgc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2voztylnj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qxhgvhaz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lrvbzsmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tyhgocaa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rgobswld.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvghlofn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ihklxuvi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwetfuku.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bksagpyg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kvdrpfnh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hwsvlbvn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bydmsuuo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2msiyiqfx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvunaice.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yubzvdiu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fagigpwr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymcqnzom.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fthfavwj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfoxdntl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eyspwbqx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dnxaooaj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yeicbzwl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blqpmhzr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awfchyot.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hrinphzy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2exmqfkoj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2oqqbccgb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezxbbkow.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2imcdpmvt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2znxgejle.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wnyzwpch.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvvmzvsg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2aptyjcgu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jfawipoy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2twdyuuce.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tdfgaysw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2najhjdge.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jikvtoeb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zcvpcoag.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tdasjqcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2goeshfbw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vrtsskja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyvksphb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mbtdelja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zignffdw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ixdnbeba.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pigtljui.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bbtmgmvj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jvcqgszp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2padvrsrd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqtjcsql.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pnkiorkn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jskfttbd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2coxcixhx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndohjsiv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vnowifzx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgxlfxlq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qlugnzgt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2avkosnbf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otpzbhvb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ecyrhxks.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gvslxeuq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhpusijr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rqdfxrkn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2flkpaaaj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ppvfndys.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ioodgoeq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cowoymma.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cwbrmzal.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rkxmowwt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qvqiopvi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cklnllpn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2upndqhfn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ommjaktj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tzklzdzy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2elejmoll.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmjodrx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cohdcnhk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gspxieqm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fosrnusq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ihhyanwh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bqbiwsie.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qgqhqylk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2auwzpwyo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybxkgvlw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2anbdasfd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2traidybq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nacfdxvb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehadxzve.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lajmorqx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2eadgehik.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jvllhlaf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eoyipnzl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2frznqwxh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tlfnkgso.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rognkuli.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fxmnlcte.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hcvrspyy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vyvstcbw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ibhxxlir.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ywykugtc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tmqzkams.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uszzfulc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nydbumtw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hjkoisdh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dmgwghgd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xavrxxty.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2norinuqv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2auhcvzjk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yydtoapt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qdwkmnyq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhrhhsjp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvqojtrh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvgxiriz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jrxhgcxn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2szldlayy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlfarmof.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2aorondwl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lzbdauqz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvjulahd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kxcyctjd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dltcbmbc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zxslptxz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pqyqzowq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qbxwjshb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iczfhtcl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jtvusaeb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pasxzqlt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2amtoomeu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pglrtojv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tplqwjha.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ueqbdovi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hoznaoqf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nwtflbwm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2lxnzguwq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jklqrasx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jtyawqpu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmwhuadq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mmagjhqr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qbjyyxvl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdsxynso.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kjxjkssz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xxlxcxuo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvimnibl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzivvcqd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mucgalcf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jajyokww.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2seoxkdpd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pbtxhijm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fseloejr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mbyiafwv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hjuzlgol.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nwqlazak.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mlouodje.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kadeycag.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tqhharxl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lbsppbui.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kdeuqngo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wjxazwab.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tgpnsxwq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vlmripht.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tiqluyus.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xgvzlllj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kdmepzke.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2peahnant.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kisvxsyl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pdfeccrb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbvfdiri.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vzhxakaq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2oypcnklb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2laeakwez.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2iiavletl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mobmiegm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tdtnmcvi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lqnwltvv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ktjunxlz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2bojroffk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2swnjxteg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2evwykwdn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zfzjebmn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pdbcvypo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wfwirkig.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2eshvlxqj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2osemttxv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mfzganwm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zibfqewg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tpjjtnkq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fcwnzpvd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tshwciuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsgxubnd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pzkurluf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epcftvlk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tsvumcbc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrwdgfq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibpkinjm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lggburvv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jmotwryv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxarbcog.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2huxkebzo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ltmowofz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lattrklt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fnduyfos.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2exazrhzc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoolnumh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lgowkbxv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtvptlnd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtkevww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2auzsmdym.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tcmxszjb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kixedfld.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ibgtnxxx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dbdwcixf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ekpcdqky.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nrlmqzib.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vmreislw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wdavyhdg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gutqcvxf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2azyejyvx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2someaavu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rrleoqay.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2pbzvdvnl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rynwmuvm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2espgegag.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2joqixayv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvzagmfj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ezfrkocv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ajgsfcgl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xdsdkkjc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxmbpmst.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2jmvdigox.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vfwqhnqu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujvzmndv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgkrsaag.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2czwpvebc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pzcbbsou.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ahpjoycw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ivfpfesl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qmncggab.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fgtnjldc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2esfbzgko.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pgaagagr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bgooobmo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2duvenejy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ffsrvdan.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2eahqcnmx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zlwcbapo.html


<!-- 参考信息 -->