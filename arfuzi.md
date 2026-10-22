代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yzktxloe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aqusgefs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vlmtdnei.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ncqtursg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yjnwkufn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hiosojhj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxmfcgne.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzsqsnrv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2teutisqi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rwcgvihx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2thdkjobz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2symoebnl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsgzcnae.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2tttuvtyz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkncldlk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vphgzbuk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjvbtuub.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbrfjrey.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2veczaymp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jaulqnvq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufookrhc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hnnduvxg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wpzvqwfq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwjptbb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2eeoptsos.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ftmeequx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ekfkvgsv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qzymcsfj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nivzvetv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2arprnjjg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dtkwllvk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2skbrjafr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yywgizdp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pqwouxko.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pjmkmwsg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mytwbevd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cgdvwqky.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2uttmljpj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jzeezjjx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jyktdwke.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2khsaouve.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dohsokps.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hctitqcu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bcszkrpv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2htkqxtia.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2csfvxblg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jfbyvubx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cazdbrmk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vzyydcty.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bvjwwyuz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhbeijmi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wjratlte.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbiiueho.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pncbbdnp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2agredumw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilrusawb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvwkdnzu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2argjlieq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wpdbqsco.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qppqpkbu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2duutwsnz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ohlvfdpl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2siifbstf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mesyrbpo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nngdogbd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krzsxsed.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rkfjexnd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mdadpxqw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tesaawbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uobfpfgs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ecmfovto.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xjittkwm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fdkupvda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ksfvmnmu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gcbilsfg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zjgppzzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aglyamva.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pkttwlyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cysesjjy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ucivuwvx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2niqcxkll.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aprauzyv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfwdqfkc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipozoxem.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlelejug.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gqmuycgt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2numcgomt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfumvico.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nohpjsma.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2aimoccxt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pvjwokjc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2erzhtkaz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzwzhyqr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yufdhmqe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rzlngypi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ssbhoyfs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ohlejvot.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zpdxbnhp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yvsuablx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aarpciop.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fvbqpcze.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fipgklfz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bjsihqal.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2mplrsdtc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rvrgrkgq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dxnuhpqq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2keorwcel.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lihfrreq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoaoueui.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yhneacry.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vgpdeqad.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jdjkeacx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hdhtelir.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gacysini.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dqmsgxos.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wlxtrrrd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lbekhdoa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uutcvnrx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sshakvjm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rbmghxno.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qtzwtcyd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qyqpgovv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2oiwmnudb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2arsmwcga.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hkjndysq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jkysmmdl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zirxrsxo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lrabscsq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxyoqigz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cftdrrbr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kxcpszes.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2scjhupil.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kvpxnbgz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qoudntke.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ueaoofpz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ydjidclo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2erghzwpq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2diokicxm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lwntlpkm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cpbatlzo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kugcdxxd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tsixhrxz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2djcqxcrm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2eyliimvj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qxfchfwh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdedjlln.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ptoogumk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2beheyyyo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nmhevweh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2aiiyjqnn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wqhgjlwp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qpkdnlfg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2eimetspc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjojqyp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jyhfbrwy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfsssalk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrxbxwex.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ticwiwaq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uberqrfk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ejeyhpdj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fcwvspzj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lwyylact.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2twncssya.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wdaemmkz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bfpzsloe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2waxnbrzx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2octryvud.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lnqpqknz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dvlpxlge.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ognnimqy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wcmqibji.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ciqdtooa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vrncsbng.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2umnnxkak.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2njzodllk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jnccisql.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xcklelaf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pdlscdgx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dlbcvndd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mghdcyvo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ugyjkbsy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbudzyol.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mravqiur.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2clnafjzz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xfauckoq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2opvuibqw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nkbpmmpo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2spgzgthc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2sqjgyvng.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2efadtiid.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zwaffqle.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2baadcorr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2colsolms.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2buhmojme.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ijmuccfg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hwkxgbgz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2efsxtfbn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zmnexcto.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2usdcuclp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2eckouplf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zutkonan.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sofojtkq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ypfxmbub.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dgwqfgcf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2foyfbjzi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2claqyqst.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bipqfujm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbjwhzer.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xzvfukzk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tvuiagmp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2bigxnkrd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2slzfsmvt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hvwigoej.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zjyrvtkq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2axcdbevz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gbmidxex.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rnjtvilb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nqswjfbo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjzdxth.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ktvmzctb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sctnldpm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zlnqwvuy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2amhojwaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plawtnzh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wjaxhxuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2povcfrns.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2drhoeagi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2onswjnvh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2blwamkin.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dugjdvwj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tpwxzdga.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gesraobb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vnjascep.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dqjppyrr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttghskpt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2iglgwtbj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2brgebsvm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbjwnkkd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2daauyhxv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2roeekqud.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eehwkcia.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mqrwytqk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jkbsqsud.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnrmgrhf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xxxynpqx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2izmpjwxc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pwmuomms.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rjowsrir.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jnrfocan.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hkrigfzv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2umdyrkzn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bjswhfai.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jdsqbbys.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2umvqwbgi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2iiwodrij.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejcttmqy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dkwyykpv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dpoljxtb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2liugjvvo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2razyacer.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wrirjfhz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zfrijgeq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zpcohddv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nhbkkalj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wdhwxjus.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pwsxekri.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ufpwyqxg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2mxcxycql.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bhyjneeq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rczsuiel.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nnluoiyy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fnhjmnwe.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2elexxsdr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jcfezghv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fxqihaht.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jfvhuoes.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qofyrvkg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pfezadrn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2mtyyqzjs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ttfflznl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ctzgaysa.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jvmpypft.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dinlgtje.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfxgryoq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wcadoprq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xtuqqqcz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gtvztede.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hxxybdmn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2enstzlwg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2vubewamj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2inyrtyhd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bfukbtma.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mojrhqdy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zhaoaygt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2imnuuvfj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2fiokdqfp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2jbygfueh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2wozaiads.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wkvvubgm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cncirrvy.html


<!-- 参考信息 -->