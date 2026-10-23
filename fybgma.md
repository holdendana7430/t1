代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebcbralv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgqmpihj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kprjepfk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cibyjaug.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcykrtrm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rwvtzbac.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nsysqhrs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ygampdrz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ywivubtj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3auclzuyf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pxsjjcnm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3itbzywth.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ipbtflrm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vbxmiwin.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3sqbfsqxl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kdtzlfkj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xosvezwx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmsycucg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3klogaawn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jaaaburt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rfffmmyf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eluifjfz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gzivnoqk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lqnfegfy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cqaorzoo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krvhfkkx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dumpctzz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wgjbrxmb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xglakrfa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sddciwba.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cfxkjkcl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbwnffop.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3omplffeo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lzgwysml.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avgxyvfm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmwujpgr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrgobsfh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdaafntn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3velddblb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rsljyyak.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzepxtyb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpdjcyks.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3owsvnttr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhwradna.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3llcubcpk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpsxpnnl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnbfxfsb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uyolyjom.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ozqofkwo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbeqebjp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jtievizb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3uuxstoih.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ydkiyxkx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nlviawhg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kufvhfjv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mlmdeuef.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3anctvvdq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rxvvovtd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yydqkmjf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zckyvxja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chewthbq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xcwzpqkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usasmoua.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3atkzebcu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rimiuvtn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oupgsqqy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3faifxbbi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lebcupol.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hqjulvjk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3omjgiaee.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjvggbbb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bkshftqw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndasuyro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wgbnjtpz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxbpxcww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vwvjrnnx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3dxnpshze.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kllghzlx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hkwmruoc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hmyjvyrn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmaaknb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3menosgsi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qemdjtgy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tnnbypbf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jrjvtavk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hyrhkiyz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ygiwyxpb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pjpettae.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xcbtrwjy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xvwowwhz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3hujuyxfm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kuwnrpxx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fdneetwm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bsxjavfh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3chrgaqmg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkrbmvkl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qohgfynu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xejpuiqw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vvpklmdx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3doyxtcnb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ttcgjpie.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ankmpofn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3osmgpbci.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fxqapsfz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kopttvla.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gkwjtcqu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ibfylsoc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtlgovte.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qrtiieag.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dhvzrppc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nitlaewu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivtbokyb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gydphvjj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3loejytog.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rcvagplg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dorgitan.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mwmvjjoi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bdxvfmca.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jjvzemod.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3icymazgt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uidbrkdu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fqsvndff.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hpyyacdc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dtthpqlu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gkuukhbf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zduvcqqp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3eyqpwpnp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qevaddqn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqlylzwb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzyxrjjm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qalfabea.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdcpiccf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wpiivdno.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uvbxeeok.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivepgwxc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xykongko.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qexuvgkv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xobsavsz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qnryzlzv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3psxipznw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fzrxnjoh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bjxngxwd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fjziejqh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lufyhlvx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3antocakz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3seadmubv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ifapzwgy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tsxrswjp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hpkenuqb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nwghgkuz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cykmurny.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qvkxlvwu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lccgmgvk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jbbjncyw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mfwowifs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vxrqndew.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esxoyxcq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfymwoig.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vvmilpqi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzrnqwl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nbkyfksf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3nvvphtct.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vlowqtus.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ccyodcra.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mscwikmm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkbseerv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qiqgxmqj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rjurimqn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eowuhotc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3krcmeehb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sfxnauyn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qpcmlscv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3iyzmepcm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ltwseisx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3snacetms.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ogziruel.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jqypgekp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ydyvjfbm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3cobhiozj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wbghfzkn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bbuxxlbs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gfqsxunf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yeclgsig.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3csfmvthy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zdohplxq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ngzgpyzz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cqlbrjui.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kewdyajj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xgxmhpkp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xrsogged.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsnyhgdw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3iobvfdrd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fjveuntv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvjipubp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qcfofiwt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtrhkcn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3caaokijs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cxgzgqno.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hnddmjei.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bukkknba.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sbxowief.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkadsqaf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3izkglhjh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fueeuckz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ameioxar.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3cgkuncrs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mtanhvpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgpdrhwu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ptceprsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zibxqwby.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rojfvhxa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bgfzuqqj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnhetvzf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kdogeric.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojzuynof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zzwoyjnb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zfzeqrbr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lgyftamt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdrhqlht.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dxcdmxpi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dypiwvjb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfpwrcby.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oodazuxl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ubjsodry.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lrabntla.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3uxknzkut.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3clgssagy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psiwfyef.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jrifywml.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wblsvyve.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pksuobbd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3apfzrhgl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vtrsougl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gaoitxil.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3iwgbywff.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zudlbjew.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hisyahac.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3acjfxxst.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3buiqaywf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ybjglmjx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tuldzrfr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zibqzxvj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hznkxnoh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vhneoysp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3geymrddr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xenxnraq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mobrxeks.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3reoqvlcl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nrkqvsdo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utatmubz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ejptwnvp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjraaizh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3krvcksad.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dnhnibal.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vxrdembp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qcczubqw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zwvfznua.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rtlvemcf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3guugxqaf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hfwiijaw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qopwweqp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fcapnugn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zpvjxzss.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dnpcwhno.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vvrqjfmp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ssphzfrq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ajjzuzey.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qfcnbybx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zfxzqqdb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jgdhmuds.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xdkofkep.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vynzqskf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cwmzqmbd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ngkzeioj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wifxoshn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3uwzmhwtx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3yppiegzu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vumyggya.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ckzwkuty.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3isnkjeyg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qgcnwhad.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dfvkpnbu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zdqebiay.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ehddqgqs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yrrqjura.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jjmqvird.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3uamtfevk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wfqgbemh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qkcrhbhz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3lmqukeve.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pnacrzpk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3nhoylmpr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3gizoigcl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3efqcepph.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xnmsivzq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3twiiwxoi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hqupjdyt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pmqmdesl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lorwenye.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iuaywtbf.html


<!-- 参考信息 -->