代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3tlzqwzsw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yaarutih.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ysgwzfxe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yfkztiay.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rwzqawfu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xnwtaoez.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3huimtuoe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bccqmubi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qijdguiz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3akndnntp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxlfouz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3auanvuts.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3knylbwqp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3oljcbasn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ppbbswsd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egelpqbx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tphdexqc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3acerfedr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hfyjhxjc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjhswwwc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyrlwmqd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rxfydemp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmllihww.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wqctnzix.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwaydbzp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ningfsqf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mmajzsfy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogtfqzzk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlcmrfqq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3meewvzno.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zyggbcgt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kukuhntc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nmlytjhg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qvxqhdhb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bziplvbl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3sehcopou.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dwikqfka.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tclzwgvv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fjwdrexm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ijghxaes.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ubmzymsl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmeuirkt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3runvrtqq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xkxcqsli.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3azvpbzta.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zkrzftdl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qomvddrn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3stwifngt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3khfhxjcn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gyanskxa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ovvkrela.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uwnqhfiu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3igiksmqc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nkgwmzkq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wdskrgtk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pleyvcrc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3svxpvpfm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3istwzwlq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vleciqko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qbybnpxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pykjgkll.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eryneoim.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xfbwsvks.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wddbgyjr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqbnloum.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljfytfku.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xubqnpom.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwwkngqo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mbjbgmgv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgsplptm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ayrtgvim.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pviytnuo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3yzjcfhmj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3msfrzmjm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3obtgevvb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dyoblbee.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fbnrtdth.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aenmfypo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dhvnsxla.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3sbniktcm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zlpprcyj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3aszcrbhe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3uqoerlyk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bapgtbrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydwsjynp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3akxnsmwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybmsxttl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3aiedwhzj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3plnhhzka.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wepsxrdp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lcfmwdov.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwvhciqo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpvacarg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rqsoexro.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3locudcqs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sxwteluu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3glxkariv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ngntzybj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eioqanoq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nqbnzdpa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bccrperc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3txeokzep.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3isgaafyj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xfbqvzng.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3knfxppba.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kvefxrsc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lxxrbmar.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cnevomni.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzcpxhjy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lzuirqoe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3omukawso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wkvjxput.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fihsyoky.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dvjlpvzo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3muqojrzw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fboypqmp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkapftbk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uypqtcqt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ajitkzzp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvwrbusl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mvdzmxjg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jagugtoh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yzcarfwd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ycjdtwai.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3odytfzwh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffgnhini.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rftdbkvw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bhjzwrwx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dljcaxgi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qcxvvqwm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iczawmhe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3tcbprclr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bpsgcmyv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3loqxltqf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcaeijgf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kezltvwj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qovondfe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqgtcwj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zxqqqskc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmqsngzy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gkdzhecl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cuniqmak.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fqnfweae.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ixzuxlwq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3piipdqtn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jlsqcdlv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bqgnjhtp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fxmhzcbp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uzhzzsep.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wwupycup.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dciizibm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xsedwdkh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qzevckob.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezcvqloa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tjtpafnv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sflqirbf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tkgpaipn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qskxznsn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kborcbkm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3varwixig.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ujrsabzt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3crazoriy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3aahxqoox.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzhharhl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fvrznunv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vuklpaoz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pcazfswv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3aeityvwl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3sqwcfwzn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gbgcophb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ebvzpmyr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lsvxelap.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yqroybni.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3piziessd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wdmhspgf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3syhdjklv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lxnuivie.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yltarqrq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ptvbovwk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfkkscnc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yvintsjk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwaethxb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cukyhgrx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sdoeqorq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rfomxtpt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3endplrnk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nsimqnxv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qpvslvjd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3newlisjh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xqjnofam.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shfuatno.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jlzrfxhx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nrsvkboh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3biszzgof.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xzvmxtxg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dcjtnwsw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3upytkzzp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3prlxpvai.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pyreskzx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3swqxzqml.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yvdgszgf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wuhtqtec.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vpnqgcuw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3alewbvlz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bkanfzes.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vicdcorh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ykxqptec.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ahxtsrao.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jkeqktyb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3uiqjrwff.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pkjrhwho.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ltbbbfvl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jtrbpoyo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mlknoazs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ivbnyunj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lryiezzq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uoxgnhbn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3apfiwmqs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ggzkmmdl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3izbhlcon.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wsdaeizj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qnhjmxkv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ewhimpsk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qisphesl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qmjicowy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3elxmgdji.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qoqashtr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ksyewqfl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cppwsfeo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xkuzehsc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rvfdqgtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhzqnobz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3eojowipf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tsbrgtcv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ryfmtsby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3pvfqlvni.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lspsmtmb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcrqvnag.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpokiqum.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckwxffay.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fdllsvia.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wowmuqui.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bnibeheu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cfesgnxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zriyinwb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gpxfltlq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3msgusuon.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbentkjw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nbmylndn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mceezgss.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pkhlyfbk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecubfyhk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uvnfwnrp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dnlbetvr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhjgpcje.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yyksuvyw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tjuiaian.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3houlrhfe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ilsgnmay.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3glgvygfq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vhensdhf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fdbxoquv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zespirts.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqrlvsop.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mficyuzk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kqueaxma.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zyqsixlc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ajkmjjfh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3inpdilhm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xwvmpdwm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwjfhlmb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zvdndhnq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3geihvwzs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nylygaua.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wwijmkdp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myjfvyqk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3wetamuhq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3khogmtcr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hgkfchlu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fqwvsupx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3utqzylnw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kbcbaxjz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bewkeanr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hbxvjmvm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3znaymkcm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3onfnoktf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3kcjsfkws.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nqpmhrqf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yxqkfsqb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3getoqnjx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hdpqmpsf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3czcifoxp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vdmrzdrw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hepfojbf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ozhnbjdt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kmklhbap.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fkfhomrh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3avcpotyh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3riinkxmb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3crknjszl.html


<!-- 参考信息 -->