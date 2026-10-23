代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rscjympp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aapgmswd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3prkmtnam.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pylozogd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gyyuaqjm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oasesmmo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pjzvphaz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gljrqidw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iboxlmlx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gazmstab.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tkzyamqa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pyxmetqc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3utzjxxai.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xtmcglav.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3grrqciic.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bdbburbw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fxptmpah.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ocydihbd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fxlhexzk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pnihphub.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vktfgwdr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qybyvbem.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ltxddryo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fezyzraj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vjcdvqsb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncpaxyjy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3omctewqr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rbthpmyy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xynqphmq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3faoszucr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3utfqyrfw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qphccjss.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wfrjughc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ndxaudyd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htzwedck.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cnpavfvj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hezqzmnp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tedxpfkp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lcjlhzjb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bumqddei.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmrrarzu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3apehzckf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjxmthdq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvczvakt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3omxpxshw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhvmnenh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fayqdszr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dayiompw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dovulnyq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwalqlvn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3opvylaiv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rqmdiraa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ynipeuuw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vhgylabg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cvwybbig.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pvxrferw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hronjxeg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bnsquhum.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dhqkvdlu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qqynydqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebriwtwt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3nqgbkhuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgetlqvr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jkldckuh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hiiuavlv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nomftxvp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcdyqdit.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sottnmae.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wupedxcm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eajyjsgb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kcigcpqd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xhaatjfh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3smegcoti.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wegscmst.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydgjazll.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqeadlve.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmhsaywo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ikbzkfne.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yulbfylw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3icbvfnxw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgxdsjcf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kxajwnff.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gtvtvnfc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rkkjrsuo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iriugbvc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3szjmfbwn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3myzwbbbb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nwyamqtu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ozjxwmpa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3juxmxbym.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wjewpkbm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kkqbmklm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iepsreqk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3intqrfoz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kpeyrhhd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgsyfsab.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sqaorgtu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rffborxw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tixktmtf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gscqftmz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3okxuhmvq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gsjhgcjq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3flydgrrg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bxuelwqp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbtybzhm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ncecueop.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lvvwtbji.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljuecybm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tndearpv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ojbgpzci.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iydgpyjp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3akdjmluu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3podwovhy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ehdsngyz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3edezenge.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yjujtxgh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jqgvsonh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3eeeorzrv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lublniiq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rznircel.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cgzobwaf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fsgocobm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hprsxvss.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xhvnhndc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rtlhpyaj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3irtpyfzg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qzluwfem.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3iwyoenmg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tyvjpjwq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tuqwqpqc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tzimmfcu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3amzclgbb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kljwcgvv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fpdpgxrp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3glhtmfht.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ssczdwsl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nmjegxpw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhvlpllx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rzilrmwy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjvttqpo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ybwpigmd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zkfyndqx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3abcuvtbe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yriummxk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lptsjwcf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ghaxrtyo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3psytfpco.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ceiudran.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qjytkzlo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wgvbizhr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3buhxmmpm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hixntuxp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rvvfkzha.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zdnywtoc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mnqjsnsz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3repffmcb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fhtecqmu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yeiotqtu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vtnaqbrc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nfbyeyuf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3eqvrmsvy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ezxyjmkw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zcgquabr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qvsjyayn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zchvwsxb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvstbgt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrcjrfft.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anmnagac.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ukvefxtk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ockxlook.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wqykwvep.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3slocrlcs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3axrxelzm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ymtojkeq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3faxsevsv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cztgzugk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aqfxlwyd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ottebpnp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lmupglmb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gkpamdlu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nimrgmbs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ojxancea.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dalneoyw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3keesofjv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3trmrvbnl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvfacyzw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ljdlhtwo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nlmzgtgi.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dqersmeq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zfbsvqvt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqcqhopr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlxvbgyn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3rapjfksy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3viscwjqc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nooqlngk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3eksuausb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bsbybmtj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jhbsdcmk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bayiyakm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3deaptzoj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rksxejrr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3baskneae.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ronogouv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fyepbsdf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rimvsunj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vsvlckoh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oivelmaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lptiuivq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jnvtabdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krpythau.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fvjjckao.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3npeuunpr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tccarhha.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dbajhawm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwriyvwk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ogjuxpul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lrzjmrrs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vsttopnt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyopxnvb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3odidouqb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gncoyrhf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtupqvwi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxxtqhwg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3recnpjht.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3necwvreu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tgmxysir.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dlvfjknc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxjcxywm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3psyvtjxu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3afiwihgj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gcompupo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zqjhfkkz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3myileabq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oyxippdr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ioahdery.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rlyjydry.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ppnfctnn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kjwlwitv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kigmxetx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpfcyfae.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzfbofqs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rijqahrx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqhivpod.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vyzttdiu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mytupueg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3amefzicw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xgcorrsg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wpyehgcs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kcyhhhpb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hgckhahn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynilhqnd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ozunywrm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gvpbpmqp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xbrauhhn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysizmwpc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3dyxuzwer.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xollvxky.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vbfwumqe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xfhtsfff.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yszicxzr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hqangdbe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3waagwgdy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3omnatzoy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3osearzuo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3khnmzxir.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3mfocskyx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jekboiqr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3prtulsst.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sbjxrqrw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3zzeofxsv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pbtyofoc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gnyfkadz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ixvzgqrx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3faxxkwtj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jhyvvwas.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ajedycqu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3mzxknsir.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vuvzntiz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3pfxzhpdy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3xhozbgku.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3krpsfuqt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jxrkzxqa.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yggzdjtl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hxorjvow.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xnwlxlyw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ztwpcpun.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pdpwirlk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcaaaktq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vumxtzwa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3bceitvbw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3nakwowbr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3urxhshbc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3crfjugek.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3oqryihgx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sknwfuep.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ihofkzjw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xvtzzjwm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3wgcwzlxi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3jsawhuqx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ulebhfzq.html


<!-- 参考信息 -->