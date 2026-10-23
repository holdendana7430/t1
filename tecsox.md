代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rpssymcm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3smqfdtqa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyxchrhw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tjxxxfbq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3arirhthg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvcyldow.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nckpvoal.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lygtahrq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxulokiv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzasmclx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3deaiehbj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kvchcskq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ekdrekmn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ygvmvuoq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ekvskpqc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pqqucwdt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3swfhlcsy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3idzeuwpe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mkrmwowh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ehgqvsvu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jyuaalyl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rasayzgw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cqoczroo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vvftufcq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3genvtmou.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jokljaqh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3syaezqgf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fglgiknj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bqpbrigc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vuohlheo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zghrbfro.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3znhfvhfy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3phvtgtpz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3popvsdvf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gwwebsub.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wooqpbep.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3hlvbqdnm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nmrfdbzh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxjzacbn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rneuurxk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsjiwrga.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vumndhgu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ntwocqzw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjmtipzb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lasxevzi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ityvkvvb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3acmapvwy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldgqaqsi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lylqalag.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggrxfvbi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrqsqeem.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eydpdwik.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wscplrvt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzsyrgbe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3opacpuhs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3osegogvw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jzvcymyy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uxmjnnrm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qmsfmuck.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bnlpnkbt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uajgxfmg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3csqtmalq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3eyutythy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3oxfkxzil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjbaxynw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uhwouhbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzbxanxq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ttdztxak.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hehqqeis.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pivwnfns.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3inlzsjip.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpxlemoz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3geguifsm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yckycxzc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jhurbtxa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtccspzv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kkgmdfvr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3scduadtt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mncnkxel.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uzamrcnt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bvijtins.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kifrfkrz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3spysbtem.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tnkajppd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljmlehqw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yzspydqm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ibdgsfwn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lecdpsck.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3diytexfx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3kjfgejjt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rdydabnc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3orybuiwr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ghlxlsvt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xwxyppwd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pezkzavs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tcmoxbhj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pwoexynm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpbdpqbc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rimjxpog.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hsswwogd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bcphwzxb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tzhcfyvy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iaxcarcj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kpacbwdo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3snsuxxgj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hrnulhte.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dniqjhup.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cwtxerlx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wfhtvhzk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3barhkket.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sxoaawes.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fujoggro.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zlpfnwvc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jtrbhzhb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrkmqgdp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qboczmzs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3svjrjrip.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdniqalj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nnxivqpv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3yaviyowx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3abywckpv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ykzposbg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3pcczzjzg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rmjnrzpl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3erbwiyib.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tkqakxix.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xkcabipr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3dzvreglt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nwffccds.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zhjsiqxg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fcctqbln.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ilzubvwb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oslvymlh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hffoiwql.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3olvjdrbg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3izggevpz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bnazpccq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zadagrxm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwczuzli.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wdguakaa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uesarbtu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksxpopgg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3huissytx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3okrsevra.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iweftywa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jvmhjhkv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ecqvxhiw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urrmhkvl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zqusqovw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3orqbgkjp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bszuuxib.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ggpduczb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3umvlljlw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3amnfbrjh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ifmfeygi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fdxtwowk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jhpgmlea.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vnjtmahv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3awuqjynw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3miizuboy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiymderi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3diefnxix.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fharccvj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3femfcxjs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3oedotjwn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3eeodahwo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fvwnyswh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vnplkotr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yhggiybu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ldyjzgwo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oyvvwavp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omuukvtz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3beshnauo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3soiiytsf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3coqmmuvc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qvgfzakh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cciqaopf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vkwejbnh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vsckvrhu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vjfyqrrg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hbrwqach.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tmiwvelt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3cxbwiolc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ipbxfeot.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lowvcygt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hqzrfhon.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qjkyvjws.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wyddklpw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mehotzuh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpnthfzk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hhjjvdce.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rsfgnbsz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qxdvoxhx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ehkdxqjm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vcjylnfe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3stuyvabb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3whkqttck.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnsuytn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3igyujrst.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvvveho.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bpyljemm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bnopypyy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vqrsocfi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pdjjrjyn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ldgnmtak.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3duzysckb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mghnhuso.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3grfjskov.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3suxahpuh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yhebgtls.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jenadwec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdtszxbp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3njjgtrsv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dvcqqurg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jtcroxdg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wogsmybs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3utukmcdd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3destqzfr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sgyovwsk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyckoywo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nppfifow.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbtxcgib.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hikfhbeq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lijgyllo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ndajqulx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oegmjjkt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbqfzedz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3glfirion.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzyaekrj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3drprynzn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xsjaqsxk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldptvugs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3enbbkyjo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3anlifqst.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bxysjogb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xsweuzdx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xdbdodmd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wqozrzlq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jmcztcar.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wmuldqxs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mytnvewf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xpyzgyuf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cjtrkfri.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxdmczsu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdadzfez.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3oktflwfo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkolyahv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkkwjbr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3iazeglhj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3eywfnrps.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3auwftkqx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zubsrlqs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rldcmoir.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dkjayxhc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxaxlquu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hwcviuls.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3irsgknuk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qgwjuneg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3crifmshz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3opgmqutx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3uhoxwvpq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zwrzdvlg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nmtkgcez.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3heefvcgw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3iperhvet.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ifmckxiy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ehjvdcmq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dskmcveb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cvugiuqy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ashnsxxt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3plhkmnlz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3noodrpzj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cwpvjbhb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lhbvgqiu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ucxiznms.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xnzuyqux.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uqgrnisb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3zhavfsef.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ppdyzkvz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zrqkmbhj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vazuvirl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3glafnnsq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jbhpoycp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oqfzbwfr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3jjzdhaks.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kzzewfio.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rorfkccd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xsuvfdyp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gwcycphz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3rrbncrtf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3djaelaiy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dfwflbto.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3oytnroyz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3khakeisl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kkrtnjna.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3gefjaxfr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3trvohxzc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3zecbwfrk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bwryueir.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nbfyaeix.html


<!-- 参考信息 -->