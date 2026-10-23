代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3slraozjw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ogffeswc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3loftuhek.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ivfvprdv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wubksdcp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lrzqqlpi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yupwksuq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcjxuoan.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ruihpnsa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uscknjzp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3treaxljs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3niyoltwd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjleqycv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3oykgvfpb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phnjwldc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qqtahjyd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhpelpov.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ryqydiqd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pfbaimfh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hznzcxvh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpugfark.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bwlswzxg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3uvkpaaep.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rcevryxb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3biptnxqr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yxbndehu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3moazwccz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ckrehojx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ggurewuy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mfclndcq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kmcbcgeg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uynciobj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3exhjcucx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dicleitg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pduftghu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hzhsbmph.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3strnbolh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hfsexrnd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ctlxxkuw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3adafvseb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3odmiidua.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbtoeyji.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dcyfhcnd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cotqshwv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3iqbykzyv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fzhklcnw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hpttcxpx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mqvptmja.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mwtufzdl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3iyqkauqg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmofifke.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xuhqhhur.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvzrtnnx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzlltwca.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cehqzgpp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evghnnrh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onduisaj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cnaxaiut.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3aozhyqis.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbjeansk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqveazdk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avpimjvn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwpfagkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vfrsixqq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ieofvwoj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izbrwuvi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ufwjldtm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kxgkudru.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3euplmrra.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3igeozuvw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3doswihih.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pjluoqaa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hzeytcpf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dtvheckm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3pyqdgqtb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wxpkvzfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcwfqoiv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mbxglqdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgxtzddi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ioamlfxp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mildtynd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3aasvsdnp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ablbzcto.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3eqkvfbru.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zzsokekq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uovmtidw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wqeqiphh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dngdendq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sjbgbeyh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kjvqmsqy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bwxheycv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prdzrfnp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfxenjez.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bitpkpvy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kxgfrbij.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ccaqbcqu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qqullbvn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kgrnjhwe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kemamkhq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wqhiwplc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3prgfhvay.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aibwsmub.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3edkfnwvk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vilagiea.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wzznwbrq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ukrbvjzi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wfwdftlb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sbdptgnt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmnffzco.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3koraakzo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mwghlsav.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lduybxhe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dknlcfwj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qmdkmsvu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gigecgjt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lxboxvxn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ukaekbys.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvbyomib.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gximsyac.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvbrbokf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hoojtwcn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ssechnqh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwbdtzza.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivvmleqo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kjchlnii.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xuecuurf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwjajawn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3offisxxp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdpqccpq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bhrmmsnh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ntvorsbi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3oduztlqs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3eygaoyfi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hytvahtv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mprcidty.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tnzhvqxl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gdmvzhov.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ziinicob.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3efglhzbz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3usffumqz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gdxiiefh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tnuhbkxq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fbhizyys.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vzquauoo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lczthsee.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xfpsfzkb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tjsssgpq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3oucvurnj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ibonmetz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3olybnhfb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eqdflrwm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3govdlklj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ynpbtkvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbevtdvq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rsgvhpfk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3syuwgesv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxcngpuk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ybxninih.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vehkgzrz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zhqikudn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jpwswtri.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qvjamwqv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zzgjeoaj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3quozscof.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rfjumsdx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fsxozizl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3erktvrdt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3txokqmgp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3weujopok.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hfeqjtrx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jooxqunf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mezbahdc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xxcnyreg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dudkqykl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttsekrgz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mkohilgq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xcdvbxua.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhfdwebn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3aaxrfdjr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gaqmzpmk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iyxnragr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yboujvhy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3feglcrme.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ettrhvhu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xjcjytyz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ywkpqpye.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wtyqeqex.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lmzgnpbh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wvgnfhlw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nrogovvb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3klhuplnv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dwbzpcae.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3egbrbaxk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dslruost.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uwestzdj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mtdnhxuc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3skdjxlis.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hwffmyaj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qyukhtgs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nutmcysu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qpadimjc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmfbgiki.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xoevbuyt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cgrnlais.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3amjfwzmv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tdafjlbz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tckkbxnx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrvlewid.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jradwrzq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vhyzoifq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fxuwiicf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3crpczgxq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3sudyfllb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xiauvdih.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yslfiehu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3srirftzj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3utfhcete.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3njduesqr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dauahyry.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qcdvpnsd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vinyavpi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wmtuqgcg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nrncqmyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynnytnuo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vfnxvxne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uchynlel.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wsvjjjnw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3abhdzmkc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cbgmqjyx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtcerxpx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zjztvhnp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uumqfkin.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3shuhilws.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwqflcbp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vkmkoavu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wwslfefr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3uwhgbszj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nafqubja.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipdpentq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bedndqtz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zazndcby.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wdzebuor.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cwkziisz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oijpzman.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mgyyrbdp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fkuncysq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bnpkppbc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mekjyqux.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rhqqjdkl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lxoqdhjo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vbfkypok.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3obxwdlar.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3whltvwjv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lcorisib.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vbkjvxxf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttmakswo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3foqirvin.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3shldwify.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3crmbfbnw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jibldctn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bzdxevnb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3cwfuwewi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wqpfngav.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ignpsncf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfidmamw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmbcwubb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgoazfid.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3yizlckom.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fybfcszt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3sjfmbqci.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfgykhqm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pazfucai.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hpxlaspi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zwfmwppo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iqavheby.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jcdvtmle.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qcqbycpz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3eduyajwr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3mwmzddht.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3txhozxyv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qoasxxgx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bbtnphnm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tkgamvxx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uvzwylzu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pgovfpxe.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lrolzfkl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3drtcwglu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pgxilteg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wrkjugfq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mzotjckl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gweatbqv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dtfafkop.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zwwszdlb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fsqiuzha.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nluyvnie.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vfwexfbr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3inhxprgz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jvnqvbqz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jopbiulh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xzdxrske.html


<!-- 参考信息 -->