代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iiebajfx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cjzzluxj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmvgshhx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfgkpuua.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkoerxeu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2syuwvjbc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uvwoanpr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnhlzxsv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pokfoeta.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vqobouqo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sbmlorsz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qrmiqqji.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2uaiivczx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wroupqvz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2foptwlxp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rlcgrqyn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vbxnlmfp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jupxgyei.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rknjbkal.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xcjqhkwg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2blrctjeq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeluzoof.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rnlimixd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kjzzystn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtuhukr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lfhxrrgc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2thdfemzu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mgxjcywe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ixfgjvyr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dufbyjao.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cvnwmwdn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cuhggiqk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nlcweuer.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2slwgntpx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vuznuttm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdeorzll.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zjzecpeu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nwmvaabj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mcoiqnqd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbertkgo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiogqiai.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gunzsdrq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tujdtvhz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixijravc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlfhrthf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdcmafnd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jwdimlao.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnqqkllc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tngyjrhu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnzaiiro.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmsuzdwc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bxllfdwy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2anqqzece.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfmftji.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xcsfjyxz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kidcuxnx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2oxbqprgg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ximxfmvv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2olcxlktg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kxopwrwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ynyxoqdq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jflfmxhw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2izlfrpxl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zykuexpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nicbkawy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pdnurwql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyzhrpjt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2remwdius.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bxumtgij.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mheettyk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pidockae.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2aksdfcaa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfzsiuvl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ufcikbjq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2amzfezqt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xlxwmcrw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lheumymr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ljyicsju.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqugzcgu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eejcburh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldqrlkog.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymjlckof.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vbcxypem.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2uwgblvhi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anvstnwi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2snyxnzxm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oiyleiyh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lscwwdob.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aasaarsv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lvamfqri.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ubimwdzj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fhmpeutg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xxezewih.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vhwiknda.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gtfbyjsd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qnglknkf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opnnbajk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ktdznvks.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fsnwztwy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xwuhpacp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zafsurds.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfzgwkws.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mvhcgvcn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fhknneih.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qjzuwnpw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lapelwqh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ntqmcsyo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlcjcdup.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2byamghlb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dgtjjhli.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmzpwufb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2drsdyfbi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mtzrnibv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2urgcqgxe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sxqrdvkm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xckjpxgr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2drtuxsbc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nhpoppif.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2glioyeyu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcsdirrg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2eetbsdqy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iegljnhs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hxzzwjkg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qwdxmsab.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xryzoond.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ocyukrfu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sgluxnvi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vntvsyaf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ntsdpiir.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2iievdmpp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2coaqtiaz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zhsrafgd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2heaogycb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wgdylodi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vwjknctn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pcnqroyh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xmrwojps.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vcqwhesq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgnwclfo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nwmdoyia.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2acfvciol.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nitzyqde.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gfhsauhy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vttouxjv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2gpbucdhl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zzntgqmb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ptzimldc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuftdnvm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hulelqai.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zrytsymv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xmxktqrl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cutdstbn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ocmxrxhc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wznisfht.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dwvgqglh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sgdmwrxo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hdicmucy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2crjmfyhy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gpcdnuiw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2apjgmndr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcgxwjkn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2scfxucxc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgqisqnk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2egzgfgyy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lscvlclw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufpvtcgx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2clynpavs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pkftbkbe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rargmaww.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2caeyttzo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouqpevty.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fhowujrs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wogrxsdv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wpavclhc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ofgmqykg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlxkpffb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2khsnyswo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lnlgimof.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wkjwhhpx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oysvnrms.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cmmzshyb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2sojedmew.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2njbntrwo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mlbdwpug.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2dwdpglyv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uwsiwakl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2laoplhky.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gcmclkjv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kehodnnj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdgorcrj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2aacohpnv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mvxisrbv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qsyjrowm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uhxqyyzp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lvxkxeak.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rutjqfdt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rkfaxzzr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jhivvaay.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vhqqpvsf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2egsijqmn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2pcimzcma.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vmpkzmko.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xqxmjmcr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jfjvkebp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ykkknfbp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhhxpeec.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ypcpsuzw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xqdphkmg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ebcxvvmm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dqxmgoip.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2umgrjmcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrtmxgxe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2khozkkql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnlaygdh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2drjgtkhu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdfiuaj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvsynkrl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xzykvtck.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xblpwvug.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofztfskr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tzqnvzoa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cdiazohy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vywwyyxi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vfokccoc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wigzstyy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzsmqyxz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ygnwepdh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fovbgssa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2racltrtz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2brhhgeqi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zamelyth.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2igchpcpb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lxtrvmfc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2cpnaoiuv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iorrywak.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qbuiuqra.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2krnqswxq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zcdpqxzz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hejntqxg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qrikixxv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2msbshfvq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jophxxzc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ixrgevvz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wosnqdbj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhkqcraj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mpxdnlyh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnaoaums.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2cbtjzzbw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bsakrbpq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hemjuicp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2baupbrqk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hunbmvbk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gjxgoyew.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rwqbuyfx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2absasbbo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iofylqkn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrupxzw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2douxgohl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ecksortk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ywdvnhdy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hugbdvyh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ylpxwvln.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eiijzbvx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xqdwicsi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2apcrfifz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2aeiixmyu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ncmhbibh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2tfijapvy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2bmhlpguy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2crjlaskk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rnzabywn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2midjijkp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2msmniddh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2bykfibht.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lpemmdjs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nyejcryz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2clodcjcx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zsqmcvnu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ebldzejf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vnyzkysl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2cjktyagc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cldczore.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vwsjpqqg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2yndlkhia.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2chaqvyrp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nsfvnlcz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2glohjrme.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2whrimmky.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2aobocpxc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kmrkgrro.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xnvpguza.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zhbzwmis.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vdbwxhyf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ahtxcuka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ctjumvuo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2zhgpqqyh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jijhhnvn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jkvuujsb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lasvhzph.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2efcepedz.html


<!-- 参考信息 -->