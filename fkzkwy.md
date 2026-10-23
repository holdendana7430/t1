代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mgkzixec.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jjxrsmgp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lncbgmtq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ruhbfurz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvodsao.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eygnrxll.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3utuqbesq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sufbdbac.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vsrlnwqh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3conxmhme.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ayipnahz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nuyyvhkp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtdvuagj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjshxnka.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iktndfvr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcyvyqas.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjgkhzno.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rjwyjwdv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yupbpzwl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfroifut.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bmvfizbh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gajokzqd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3umgdnrcl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snlsnuxf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zglaxkrb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xetpkycc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xntcweus.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xyvwlgns.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zumgodcf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qvwictbl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kcypjadn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3snckhowg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ijsylcjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wmhktkcd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kdyohppk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pxcyumxu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bescrppw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlbsgzap.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pqflknpm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3matqgckr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3umhgutoi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ncytxrbn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3twtaddms.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xaactild.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vqcbyfyk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxzlspcs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqphmjup.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sghvryvt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yuklwfpv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iyfceltk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hgacvosn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npquqyre.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wqkzqgur.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3roqkwarm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbqiluvm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nievswsb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blohmgku.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oshxonwl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lumqsscj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjybqaal.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orpsbzqt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tenbupym.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3sekqopzp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xeckqujk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3flapxvtv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntbhopol.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufreqjff.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3iexakvgi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dmkzycsc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ireazxil.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ynrxjwdj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hvlopuzo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3otxhlmaq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3aliubihy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qymdoqfl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3faxmtokc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dxephxzv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zetegxko.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dvwzezfj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hfgahbpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezeijwxd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yjwsdkam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igebifoy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3oxxkttic.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dichlqqx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbchmbgb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3axatfara.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fottpapa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3okpmzvuk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ejgjonqg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3byevvqjf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3smnookgj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3trgmococ.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hqgivzbf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nnmlngju.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnatgdfl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrtveohb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3byhrrjln.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ngxfilmw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gxtrohff.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grzudpry.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ofkeuqln.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nilipbbk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nygfefpn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bxemfslm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uvpohvnq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vqpaegzt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tajuadmr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pdvukkcq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tedlytvj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rytjwnbo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kkjeqzzv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqttlcrj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewfeezeb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzdpmtmt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ncqfdiqb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pbrcvfha.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3brkauhzl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3keoxqhvz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pwtohclg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hsazrbik.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3udypzmpf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ffmylvyj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3snwlvlry.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3unwpkpwm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dkxsgirx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfzyjgys.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gndbfsnd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vmdzrljb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3iujkoufr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mocycutf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpcjcgtv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlutvwbg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqrrjac.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tlienwsy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qbvzbbsi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3eonkrese.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wmdzfglp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jbwjtkkd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3desfjhzw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iemebwjt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfrgsxpm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3czexvytt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zfqtieyu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hjcehzhc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rtjqepeh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ayruqpcl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ubegkulz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3twigkdcu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cmddzmxx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3lujdllxh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3alyglngc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3phnmsfuz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rdctvyxl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nizjrtci.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3foprhvrw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gpmubrrb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgvapxud.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qnnelbng.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3syyxcxfl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esnglpwi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kkgmusdi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vdrijvig.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3shoyslyo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3olyjotaw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cbaqmhlg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yhjdjroz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mtscwwni.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ikmxaxyr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bjvmtszk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zbdobqqe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ikbpsfwm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ggcjmcbr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3uzdnrewh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wtggykyu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wjhrvmyr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ehhopgca.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hbqawgjb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hbvpumow.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bvyqrzqk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vvdrtbmj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sopbiffy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxdwrsxh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mmzbmusy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcgtbztl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3frcudfto.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3crghvzwq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzrfehgu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qulbxkvy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tvkaeeiw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aacgjtor.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3glaanput.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3znaskupl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pukyljqh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rxvxpekq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ueinuwyy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ahyoyala.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3oljrcjyn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nefyburw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fbkxjnis.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3tpzejsbt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rtxhbvef.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rtiquavq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3iaukjmpd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pxvuxagr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3imvarcgn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3nuulxxbb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oihlwamk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3fmkkjncf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gdjyzyfi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yotjzhhp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3pkevcpiy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lewygcqd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qysoognz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3nltsbljf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3kmajifac.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3etoujylx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xtalrhrf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hfpbwmjv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3clrtdxqr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3mamjyniq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3njggwdcl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uindmnmw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xkktlaml.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rexnunrw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mflprbwe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3neifgsor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3curwsqyx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mwmyrznn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lmaftxlz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hkjqtmra.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ikfcwjde.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gnhtswmv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivmrcqyn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ccnukpgv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpjhxgef.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3sxpmpriy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3bkecbynv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiuodlta.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wypkbfpw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3juchnopc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3whwotzrt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkyalcqz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycollsaj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rbbtvvtn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cplwksnt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zigfxzge.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dcvfxtbt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3sqoseybw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3clmvvtjh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3berxufdh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jkzpjksn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3znenhktm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ettoigrb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3neqsjxyg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xuuvjhfu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dcpqqhbl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qwwfwgok.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dlhhecdr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pymeghhi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ulvkpeaf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3diqofrvy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nierjzat.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhslygi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vaqyfypc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrzucjhq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mpvbghim.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bqdqidpy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3siltflpr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nriokxhg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qyeyqsnj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irbefsrj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3eqxghoux.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gdwipdne.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kwifmsye.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3oaafqrxm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hwcseapq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uhagsagk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3asqbfdxv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3elkistid.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cqtwhquk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3siuuhijc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ydehvuxr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kdutszpp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hharpnzo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lfkytrta.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rjawopsa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iltrzdul.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lfwnqrpr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tfozpvll.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vwvotovm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3sfdhpwkt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ssvpauqe.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3krdbqvbz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rxehkoab.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3egmfccot.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3edotcmqy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rmypvsdc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xxfqfsww.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qshrfavc.html


<!-- 参考信息 -->