代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kliixqsz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdhuqmat.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zbyslbxj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zoigfxgq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmdjsrge.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rkxcpwir.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3osqhmxod.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fkolljrq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3sphvonjc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cedfdube.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fqsmglto.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fxbngdvt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3eencgvwa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3umpejart.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qtykmyzx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yovysfuf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fmcevoez.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgiutsem.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rghoadzv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3axucbjpk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3axzubvwl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ckakrrvx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vsqjyruu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lxxecoje.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eilqqqif.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wopbhwdb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uaeryfuy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3urjgjcyr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pbvngyyq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdxncbrx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zjetnbyd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewovovrr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kokdbexk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3tbxudfue.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agkhlraf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccrffkje.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcjzmbft.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuzmojld.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kyqpofcx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrohzsve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwasmong.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkcyorme.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3eedcitgp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmqfajv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgwrxxcv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpmrctlt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sakjziga.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3leomdqzr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tqstqxpu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqzhuqna.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dbrvefzb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ihmuauym.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wpmxgtbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3esmuazga.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3certscem.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3envzttqt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ahvjzzum.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rztlawxr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3larecudj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kiltfrtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dzlsofuv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3bnuvhkep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlgjcjgg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pzfpkseb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wwvgrdse.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zccmnhvj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lzelsgvz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mtcmzwsp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbkszthr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zqxampgc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tcqdjhfv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iaqoitgj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tjxgocbk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fpheesng.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pysnmyqq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lwzowesx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfobvybn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwghyfgp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wlupvros.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdgcoqcu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qkhyjkfd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3grhnyqsz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wjsklaag.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sipzjpkv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ynrbjpoc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gywxzpxf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ubfzxupe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ejzoszbm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3acbxqmfa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3iprcfkaw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rryjezmc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qlezsbno.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbdolpnu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqcwhtxd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvnouzad.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edoxufgk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ovlhdltr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdflpyyn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lkrlvcsg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fmxilixy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nqpqiyku.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcistwtj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ouhnbryj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovsiqbqn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjndhjmo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yocfmdxu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xaulojvt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hxdbxxkk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3apzyslhx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xeloakeu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cvmsvdum.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfmgwhgv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3idknegnp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqoysmbl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3idfxwril.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3smdsahrl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ucpuouak.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qvwapgwl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3azjkvpnn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3colbrwyr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lrfkbzay.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rlneszsz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3riqoteia.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3azwysebu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ygpglugz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jzvlavzb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ntbgarru.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hatwvmoq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3echfirzw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktayohqh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nvhytzys.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xrcamiga.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vktcpogs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zcrfvkdt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3agnhsarm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mqfovfmj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3beadnkal.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzvepmcj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3covbfcid.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecbafska.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nemiqidu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vhylgnxd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ysvmspib.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsozznpf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cjgtmgto.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3drvvqrgl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cfubhkzy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gpocpbbw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sjkvjlro.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lpzfkhxr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vzjhpiiq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ncgzhjcf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dwmilamw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3avkbogwt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3uvxxtvdg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwgaxhnv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3benmbbld.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbcqentj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoipgbxg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3akqcqhfc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tqestlnt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kszlprfc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hsvtbktl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xsrksmoa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pgybhslm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dizopure.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oisuacrn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xccdteoj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jqurlekk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ygksplub.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yhsrpjfi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwvyzyal.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3tgylrerf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yvxuqocq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kgcylloq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wcjslbrk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mojjtgoy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3oexkrzje.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vecckxgp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3japxhpxw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ohnevtbp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wnudynkm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3irfewjym.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3svapubfx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wtrbeolj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3smkgukos.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tiraegbz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dpotdkhy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wzqsxche.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gtpqkkno.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kssfvxyl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3epvcsjch.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kzhjscrk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkajsrl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yavcxdwc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3tjuwpjul.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vuqvrwqe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lsbcoezs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uapdyvyd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lidctfvo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dfpnbcyd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tznjpguq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fvgymark.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rambbppg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xurueups.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3iueoxese.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vlmekzcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxvkiqvo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3twshdayo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exotgtgk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3eamqjxwk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sqifpzws.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ermspfcn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iznjkltp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uklllfyv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3oyfxipdu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cuwrzuoy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3njxiwlxz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rksulcxm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cppuaqqr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pjmqxmha.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3esziuilk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lodhshla.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpqhaxic.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwmufoxx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mdjluyzm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ismmjzaz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fbsgamwh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xnplhwsz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3sdtmjzck.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pdduxjxh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qvuksdgg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3chbuynhz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vdfeqmep.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3oryzqxpj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3onstesuu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zanttenu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3gfagzhmi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uymlxxsp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yolpldgp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bokuwgof.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3llcxcani.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zulhqqhs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmnxvvf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3yxeptdne.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrxashyk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbuihtzf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iftevaeg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dyrcelvx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ktwgwwhz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jjavftly.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rubdzpsi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gjdsynzr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3rcpxbyrn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rirfqxiw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bmpevnde.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bvokovou.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wfnqxmil.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3enkuwdrc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dwnoxyrh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kzlhfyui.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xlnpzdpl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzuktzex.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3plhpqavp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uceamzjx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3paktbkwz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wtxzkexf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3btjyodqn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nruyitbo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vjadnjdp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3okudetqw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kruytjlp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tibwehel.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qfyogtwe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tjamiybn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3nuavbdgo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vdoynalr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qnemmxoq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mivrgsay.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3rzfijwzz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3gkvuejec.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gdspnhtt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cvcycgox.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nxhvpyze.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zvvzemhw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3cjldxnam.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zmgpexqf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfidcvpc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3lriiiqlk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qcnnauxn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3axxcucwz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3prjnjzig.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fptorswo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jpprheqy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3okrkxxkd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dccjgvjx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gafalukk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ydejteas.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3hkjrxfvz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gtxlhmxm.html


<!-- 参考信息 -->