代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rlcngzls.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ideuoveu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fkgydihs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dfgnpann.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ufpflant.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rpdwvuns.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fydabkdr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rpaydofz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3diswwujb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3csltchzn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3opjhbjts.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzentqja.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3malkszcf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3liwvdqki.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kdqcvqst.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgkrngru.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnnzcgsi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rfwujmhc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbdypqhm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xtfdjflj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjjbvckv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgffvklq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmnrqhiu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrmkuhnp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkosjmbi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpexxfkq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dsslbavp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rybngbal.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sollbemg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3apqvnhis.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fbtogxkx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lknoqcpa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rvqxkyiv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mlegiror.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rkwfwivn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jqlltcqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rfxzkvsa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3potfavkv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rbmpastr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tekocrwb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zzjlkomx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3juuyisrr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qzujzthr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3apntvesh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3iyftbqqi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvfjgkls.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ojbuotft.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mzwrxtrp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nltqvygd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwpjomlf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mqakxxsh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fikqotwk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ketiqfoh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jwsqwfhd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocfciinz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cpfvnmpy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfyduobv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzkwxihj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cokkucre.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olaixywj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qiqjiurz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3goejdqzg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tdivwsdh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qajepjbv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qtuwpsig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkjgozrx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tawsuasy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bpcicvyq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qqwcgrdx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsdjqgsc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqbghsn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jaytlalj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3oqjrlsls.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yllqunhd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3iyfirzti.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ctvaidrf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dbjlodyu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mqaqhbzx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zpbqaril.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3amdaqvkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lblwafap.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3apcnoyxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zooohazj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vzbbdtwi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fwoolfrg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjtgssmy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yuoctdby.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrajbcmx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zmtgnutb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xlwcnuzl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dfkkvvca.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssrtfszo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxizybjv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ooohmvwk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dksendxt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnojebjm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jzrfalbo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrrbygwf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hqfipwpa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rjxzmyiq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3goktkheo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rahdzscq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rhqaowph.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3moblyvuq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xgourqrq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ftxefbva.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3uxmnjnnr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gyiomset.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3druqfili.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mboojemb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3egrhfwil.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ihtmmlir.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rkfcmzwp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyoabsnz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pghbmqcn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bimguuqd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jeokcvdg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bzsetjzw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bjamknmr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3sidmmmwr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uyerfzvd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3galjppbs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytkrxkxw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwgocmem.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hispzdyz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bibcaczb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3stmxpxsb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3sldprgoa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3srsubkeq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3yzbpwiof.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uclteznc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dwhtjbrw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbkkxgkv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qpwwcsxe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3celsnaua.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbwvswyf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qveucmes.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3emecbcld.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fgmomreg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vvlhbtkf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xbfsekoi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ytujocqf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wbckzole.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mcggenss.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mnssfjyr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3dnnhszai.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wfqzrfip.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ytsatlhq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jpwtkecw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nkgemrdl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3soqefelz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ctgpmklh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bowvrskz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nchiczzk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iggkhnft.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3oygdcwsq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bxlekljx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqwrkqyj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3auawpwvn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vgmanlan.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3esjblsux.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gxqizume.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3slcestbw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ochrelqg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fspvbici.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vxwxngob.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bmztdwqj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sshrxvoq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tkweovlw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3umlclgoi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ilskzrhl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3swjawtby.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zppxsawy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rdkmaqra.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oiptmkxi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esystmiz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tlzhvrnb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wkshlhew.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjypzkkr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zltldzra.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yiirntmu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kucpwbsn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zhhovvqs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ddkxstnn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vuhgkqky.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uvkgzegu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sqyixvaf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ibdlmjlu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zaperyux.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mqwidtun.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ehtgwygy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jpnzsicy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vuatshxv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uhnajwzk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3upddinjo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kcvjhrhf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gkkcjejv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cuctnqjz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzudtla.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mrlgnayg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ifedmkab.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sxotioog.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3urgwkbrv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3sgfcinkh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bdmlngpf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vjfqccwb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3coxvjsbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3axivgghp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dmbehohw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3loenocle.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsnrwvin.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ahimtgdz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xvhdyppw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zhnsbmyf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jatbxner.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ajrheemx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gseakmyq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rrinyyxv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3urukvrqw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xaueulpl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3iawopmef.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gogpxcxg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zbfrgoer.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ogirbxmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3pwhmzfmv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3iyybacuq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ijntrvpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sliddfpz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3obrdqytl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vnbxjetp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ftxrhcod.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lmmfsjzd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgcvmhvo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uqycjnua.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3flasigzh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sejpygft.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3youaarnt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bhrrvfzl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3twukikqr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xufiplwp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3yseukmeu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxhmhpjh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pmaltmgr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umoiqcqw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aylofzpm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ugksekkz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3irohuzjs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3deoccqpd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ocfvbuxi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wdbwbvqb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3asbwqaff.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dhhdajzq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3neyfryki.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fvckrlft.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hmqmqptw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3sxmevzxx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dqmnhrjv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3krmmyfpq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ulvixzmo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3oalnwehj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nshplogn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3udcobvtd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3idtlnnrx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3nfiezkeg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlwrzskb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fdwwafbz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3fxknywjw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gzcvzwjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dkhnttsr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vawptthp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nhvrqcsa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ingdzenu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3skypeonf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mpvmgetn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twjtuxck.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3chxrkhpq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rdefifvg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kewefujp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cbavfvoj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gdblauaf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gfibcchj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mpmtrpbv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ewgdbwgb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3oqyvwhdi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3jqetwftc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vurccbxt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ypxabmuz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kbwfkspt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qhppmdrr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3gsogpods.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3otbwktwk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hitmgvtk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uizyycpf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3feydcdnw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bqzzgkxo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3aejcnswg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kxugxztl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3syswyovl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ulqonjyw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3cdjzdyoo.html


<!-- 参考信息 -->