代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3erjxjvfv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jdeqtmlm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zebzkqov.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxfgydvp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zxbcnokm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ghhzloos.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ksjglupn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ntpugdmh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3npfirrdb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3edpnunww.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3awjfdgcc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fbmiajhq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zrdvnfnt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gmgvxxqz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ofdfebie.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqhthvdp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewoujtnu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3idrnpres.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nclprqji.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdmeifyt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iadlbcwp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qgprutbz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iemigivr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aroqqyco.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgngorzo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmawgfbc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bhdjtwfk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufhauygn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfssgqhp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3atocucuj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mxhomzjh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wgxckmaj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hrhhypaa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3abvblzpb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3spbewwyl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3upqfbupu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ppxctnoh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kprqipng.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mnbldmyu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nyyfighf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3inrzpevh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3riujfxgt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jwijrazg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nttohdyu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rvrwamse.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3etwgzsqc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dmttqxml.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xlpucscx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rmdkooru.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quwuebhp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wltlpjkl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sfiptxst.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ksiyqpqt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ijdqipbr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mwfdypuf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgzojisb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3oluqrzna.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gyxtxfea.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lefsivos.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3omaesaxk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpkmfxez.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjzxhght.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dyyhdxlq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyxefyqg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtunbysy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3smkyxtvb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3uxczbmps.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wowvaasx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vwaljacm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tmvhuxja.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sukekidl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tskpvbtt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gplsxtiw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3desrrwwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3godwyvyt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3oxqobnml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3keiiceiy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uioqjvkd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gpwelgns.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3uglygfsg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dlhwobod.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3kjtfeqvq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gihavrcf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qdoqrafh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omuyrron.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3enjwqtrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qcdnprpf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cyijdbyb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dacvtslm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3itsizpvq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ayskqklq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sswlhzxh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3egzuztfg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ebbhsfjl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgzyzznu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbeyfxmv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppnpcjgf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ipuvuiyl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fgyhvskb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aadvbymq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktyjrowg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3okevulww.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3poerpcuo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gvbpivbl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3veidzuau.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dxoyibxr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kuhdjkvl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hfvjgdvx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mwxkszmt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zbqukpcy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3htrvgsrl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3gazgtmrz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ypmgrijq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gpphbjvp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3prdntltb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dyfuemsy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qnjhaufk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yxksdvue.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wolncref.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3geqegskk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qxwywjdn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpvzthuw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uwnlpkpb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yyufseei.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xmnvgytg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jddshvpg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3czaxxlyw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dperewrn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hrlnsgdm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jygpvmxz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhrskjfm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3weuyhhhd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lvyanhjq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3dnouefou.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoqagbee.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhipyznk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wmtxoccy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhdknrvn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3erfisoxg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lgwvlqtk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vzkoorsn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3eppgwdxd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cawuahln.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3khevnafm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uogoryvt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uboqtuxw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nlaaedhw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3whntillv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cpyvegex.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ztibikcg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qllnljdu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nmizlzvd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nnysiutw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vumtgrvz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkfngown.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzfgxgez.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3geagxvsk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3brhzuaii.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3spnadxzm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3igfavqzn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qkjamihv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejmzhjop.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vvnrojfu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3noafzsek.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxustwgu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3luvhzbhh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ixwoctok.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3igkooqih.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3odcpfzzf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ioaghtjx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wsceszqy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fjdnnurj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gntuptga.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jlyzeknu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xldzxnqa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ypxladtb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qhqxtylv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bwimpvsm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3agwoqyvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eovxqrdy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sktfpuuh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iirfxywu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jvlfcsav.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xsqyacsm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3txbddxor.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3uynonyqx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qofncjmr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tvwxurqz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjeabpsx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxxhqqdi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bmrliekl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vugstrth.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jhpeuxeb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lxwakahe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tvlbyjxw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyxsoaws.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kpwezfaw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndkcoqah.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gmnoajal.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3scfizych.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rupkkalk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qjxmpsmb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3aybistix.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xaechwnr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3memcdfur.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xnfvamhy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3svthkuid.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3efrsbdln.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xsvkkytb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qeqwevhs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3htaadxvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dyjisidq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vtssltoo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nbxihovm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fmiejkmy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxlrsyak.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3iepoydmb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zzymmikj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3usohalbe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nfwtgvai.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3gkwojctk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ljlysvef.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lxkjvzui.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iavjerqv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bxooqjgm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gmgsnsis.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fecjhxbc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wgqrfyjs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xwyrhcbs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mcicwmte.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xfgwaqmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qifbjssx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3parrqjlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arsiyxfh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gngsfjkc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sersjfqn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zmxokdbq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbxvroce.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vqrmrjew.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrcepbqt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rpdpmzcn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rlmvjgai.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpqzcnpd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rlgqtaio.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zecseyap.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ivnydyib.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3somqxdyx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vsiwihbo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3snmveone.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dgheluee.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3byytkgok.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ixrqvjhm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vmoglpll.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vssqpqkv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dnczfybp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3djhveoys.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mjdlaxrb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3axjjrzvk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjirhuj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jiipfsab.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hcbdkxij.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3frgiylzq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xypkwspc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeqkmgmb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nvevnnqc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wqfqhutm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxfkprlb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vcpuwezf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgbfltvt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lpqzaajk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3fhjisafc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vknwumey.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3srjwtyph.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akkteuxx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srqmzcgv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3upwioocs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pfelzlce.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jyhitpfo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pbrechsy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qivzchug.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3lqzbabzp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tdiqzftx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lstpbtkv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ctyljshb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ifpxtkis.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jsmnsfpj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3spoulegz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fqiwaaln.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3izkhlkgg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wtutsnza.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sgmobsjy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ykbogawa.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bbvstnyp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3knpmjtgg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xtainict.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3lkrzqlzl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wdwgtedq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3veszoydh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kbrhifqz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rnixykgb.html


<!-- 参考信息 -->