代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lcrozknh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljktyeho.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3arshjbyp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lzttnues.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mnftxiej.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gztfztdn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kjwoothe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xgprpdbz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gjbsbdik.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hzqjkdsj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3apahvuah.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kowooxmy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hftdcxdc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jeixlgjz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yhrjyquj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3phwvdjlq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3trqxwydf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yrqqtynz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ysvkdqio.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vpunfqvw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kmmfzorp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3gkkkzsyy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdyjrhjg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckfhekex.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgmqhlbj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lxvylmdb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qxkiwppo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smsgrtix.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzhyfxwy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gkeiemoz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eglujvkn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aqynkneq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sknznjbi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxvmfyxa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ihqqqpff.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcxuthsl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3unohmevi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ohlkltcl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3frgpdwup.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ezerytij.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kzbqxowp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3raznzvnc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hqgsgiuf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ryihnjed.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ybdexfyg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3stawmohv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jqaakoeu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xzgxhedf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ogghnntc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zawerkye.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hmhodaao.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wkilwugh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gzuosbxg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fxlrkuph.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rmbnrrsz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zidxyzyk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hlxphljw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uswglguv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hzzlojxt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3etpcavgo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ofjlfylx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3arodudrr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hedyekck.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmvputme.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mqfxrjhm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xhvsjsio.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnjyxswn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fjxyhqsl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqjqnvoc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhnymenu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3uuyjfdqm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npikhtle.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvvzlpid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ethdwwry.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3krypnwmk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzjczqba.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3isiwaflv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pecbybcd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuzwkqng.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbhnxhp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lqdpdzgu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhikeubj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3svquilta.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3oirjwabc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gexwtjyy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3loijerlv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jxpmrshw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xguiuowp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kwzegrre.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nrxeqofi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3omoymkmr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lgmmfeun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrpzrjup.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3svovxiaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrkeisbc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3adyxolet.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3koowxryo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkndkpwe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqyoginw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pqdvbidl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3chacpvqm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fucbcxlj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yejoqvww.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3satvoard.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hkyloyzm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qrtcttrm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tbrhkcvj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gknzkklo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okqkvyxw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3huhhvstz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bvlsrtbp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tgkbvwqb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ifrwjeum.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3apargqtc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jsvugars.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qyhqevoe.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nuuiaofz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ejpsoxwy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hyczxhql.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3usakychs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jbanbaeb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pwabxiok.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3amamjxwx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xssknbtl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ljtcyqos.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tfiwptuh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxmtgwkz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndtibhen.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3efzgqnha.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3irrcercw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dulghwui.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kernabch.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jmtxlqmt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfdwetse.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3npfzoimn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bdgnmxsz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rjslliuo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wiazqozj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3flaxqdiw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hmkcmvqf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hftvxlbp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3sfkhzxnm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tktrlznz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fgprdzes.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3stojzort.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3obrtupcj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qsdsrbuc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjoqjylu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dubtrjri.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3iewuajim.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3keoelmrg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yictffij.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yurdzvjc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ewrrsepp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nvfdnxwo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3cjpipybh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pqzzkxdu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ydbuphcg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vaywtbyu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zpephpfg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljyrqfis.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdorlwhc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdxiifib.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aefivwfx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ijrmsniu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihjhhqjx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yutxpoey.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qtvssfcp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3eawwnztr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kewxtlgb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ctzygssr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fqowvgfz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wdriybqp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsarych.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xjdfmjez.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ldleblzy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zixvbxju.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xraliluc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nkilhnqg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xfkofztv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nxhqkqjd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ifculawz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nzvpzvzf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jbpmyiao.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ykmecotj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3lyqruzrh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3czfswexp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3janakaui.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uujzsfma.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oqkhkxmw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3saeepsgu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ogpibrej.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zgjxyfjq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkhbkvgr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3utqrmqgq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ewnqyyya.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehwqckhf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwzzhwjx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zywqakdl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yuawxowz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3snkxbcbr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlwpjlki.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mymanzjt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3apbueycr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lufsrdvm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fgjlqclc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mbtfamzi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jwzyzgjj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vdawbwtt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wfemdrfm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yymlotmn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tscfafdg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gidlrodn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3virqvwdi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tghvfako.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dqjqtcwr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3empfbiuc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3igwfduut.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sgfdlwas.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gseqobaq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yjnosriq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ghavnnwt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rvunypcx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwzgzdj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nrytsoer.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jyffceck.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wlxtjlsg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3yljydxtk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3burvgnyw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eedelysz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ihxoydiv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nuehpccy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cqqtehlw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cktotgzl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3huevmjqt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ssdoymhy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3orimhsav.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mhdtqxsv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mekneixd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbbbbfju.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oxgttxfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfznzocq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fkewqjuv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrmdmej.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjpjcpoa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pelkrdiu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xjcqmxvw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkczaumn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ldlcapif.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uppwmbro.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kzfzyvbd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zdrbrbhk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bwfydpim.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3temjmngh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hpznyfvt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzqsubhb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpfsmbst.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3btigixjr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tbyzqtfa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vaoivuxw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zaymxsog.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pvbfkvkv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3etqhzgfn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rjkmcris.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lqwbhwft.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uivxnysd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3nqbgdbup.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xjjxgixu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eckisjce.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3yirjwati.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3skrxhduc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ozvvaatg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qosnbcqf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lexuqsqw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuzsottn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3yaiusqhu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3wiojoqkp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqyanlnl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3texqnohr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3huqflzaz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bkobybir.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqqutscn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whnfwpec.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vicvcunh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3malssapb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3odovmvuw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cuscujly.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lykvustl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vgitmqrs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3feajrkio.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wdqbyoxe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lbfhxcoj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rcbybfft.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3gprvnhru.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ypucikfl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3fvqbmxlg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mvchkfdp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3hoflvnkc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jbktgiah.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3odamfrcf.html


<!-- 参考信息 -->