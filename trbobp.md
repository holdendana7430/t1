代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2xwtbiyol.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2bmwnxaxd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhrdfptf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkjmabcr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utmtwfjr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gzoxxgkq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ujzreyor.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zomexhjl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiyhxosq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbgzqrln.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmfkmdul.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iiqgvknv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uspficpz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdhrtgdb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qupgghxg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jjbhgocg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmucepye.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2npknuspp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bwqgahun.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2azojythi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ukuhmxxk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lwwbakgt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kqbdtmyo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wvqisotu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2omvwnujr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ovgedqyw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cfqxrjld.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zcweveeh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqqewrv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctlzcwgm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pfebmerm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2flgjyucj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2knpktojp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gdwdxxyp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xcokupux.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ykjedush.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2tppuhsim.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdzgtdhj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmavfszh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bbvhicbr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2woaxozgb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qwledjnu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2okgyfoxx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdaiievn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2scoktigw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lyzafovd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jawpoway.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sveafoqb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igqylhtf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqfsszih.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2oxmahmrx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqdebzyi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwrgwmrb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqwrgvzw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qlkugvhq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilzppgmg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wlpzlhzt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkwxkwzd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnuydvse.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkzpvggh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kizbjfrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkbsrxpu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xbojdsyh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mndpqizj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uorrrxma.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hvkwtwti.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qnpvwfhl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zhrghuiv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pxrvjhgh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2aiacdkll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vixbrwlf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2sugdnxmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmxdxhpp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dohbrksr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgddgtdc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2btyianms.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xzlzevzt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljdilhzn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgnybsgd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xxvqspzg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2axunmwah.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vygmzyzi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tuszddbh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mliowuxj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tuaznuta.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vuliayau.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hjaguqhb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uagwlslm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ffzwyckh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2awmgaotp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2oysditat.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2aurqytqc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jjkkqbch.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iguzvsru.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gkpgbiaq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bcqhmrba.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2adbbshyf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ytulxsyo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eykopnxa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nreaysnm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dfwfiewc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mzpolkjb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ojcsvyvk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zrjbztbt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uslhozkp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmvavbpp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guoviqpf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syyltrqs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hmnwxycg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oeclyzhv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2intmqxib.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gzyffjvr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eeukizya.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2opfklbpp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uunagzru.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xelwbyfi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2okdyolqh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dgrlbsfd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sbbjzpuz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajawtzpp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2aocqutrb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jvoxtrob.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfrqlvno.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urdwqwvm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2swhwsgdx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kkfbonqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2osocdpqo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdrdwrqw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cimfixwm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2epjzjpmg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pbirhotw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cbzuethv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2usjnudxh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2emwgjwvm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ojfztkzz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lvnnidxs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vpsegzhw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xyuupdaj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fgnznwas.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2upytcojs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2laykrhgo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fggrremf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zafnzcko.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvijuyow.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hwizqlzz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fodmiwvw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nincvtrx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2neqgtkad.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zxrcbhxi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxhbrxpa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hpbsmcly.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrgmexai.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tplgxfsu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2iockwycx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2edniwojo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ojledniv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ivysubyg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2avhdeaba.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dfbnmvsk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2avnuitug.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qscyxagb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nqfaaptb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kvetorrm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bnaumrle.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nyfgivsq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2twqxfzqo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kqwsyrxx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wrrchvbd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knphdibw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vloczsnx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tkehjzxb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2heodzidl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jhnuhdie.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtrfmslm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qktnefzl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uzjewewa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkaiektj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttzhcqbv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkfwvdrj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gmntgmnf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hknmusrd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2szvgtotx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rujerddy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2oiqsnkpm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fmffahgq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ccvwqrzx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ystrqzqc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nhcraitl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qsctbgwq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qydmbgzj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2szghacjx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kpmutiqz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wtnuzeoq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ipvqtskx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2gevjblkj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vvxocyhq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fcphwyim.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2icufzzqx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2aorxwlkm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cianqede.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xmucdpji.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kqjeleun.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zflikppd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffypazii.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2znohanrx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mbomhmzo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pbrpovho.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvxusue.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vjvkrjyj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2covbwzeu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2pehladgf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hkhihkiz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2pthyueld.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zqbcffxc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vgceplho.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2bhaqyusm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2nosvdena.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2juqhghzx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ihlhgskx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcwbzgli.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zdftdzjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yleugbyg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gbxerpzv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fltxzkib.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yoffpruz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nmmvmhzl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vrudsttz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2radehohq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2txirmdau.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wtwcodsc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qmvnuubs.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vodlnqcu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2vjrupzit.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gktpsfpi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aeordwrb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gooljnmz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsniphii.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lacwlhvs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vcqxitsc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aaqncxjn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sgtutfwd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hpidbxst.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uotlqday.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hmqucwik.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2htppjcmi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rghggeuh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2uptygrvg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jlpegemm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2arujboys.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikypeowa.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2udgbtvap.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nzazwuss.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kocrwyeb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2abnrsjtd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iqdlyeqh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kxksxhjv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2fturvlhv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsovwcvh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jnyzlnxy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gnfzxfcn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zlcgeijz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgepqxmw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yhrqnhrl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlzblxnc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vphvvvmt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hzipoqjb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmhmpomo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kvashnak.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2yteixmrm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rvvpsvxl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xhuwtuww.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xmmtmqfz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tbocviaq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hveqwbar.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pizgvejl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ngkyxgbn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xywkkkja.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eoyhxnkg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lpltzmxy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nhooatal.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2adgrdasq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uxqwhjfu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jqihrefl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gvfvsiyq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2glhbkenf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jptdxhow.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2odeffjds.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ndivamds.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zdhxcuig.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yfiaaqzd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2yhbfobzm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gginqhbo.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lulspurv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dwevkjov.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2vloagfvw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ttqvxiay.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2evtzfvez.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2tdekewjc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qmgqywfc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucyvvonq.html


<!-- 参考信息 -->