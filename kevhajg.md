代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gwzboikse.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gwkghqfvz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/goxrfvlzk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gduvyjqde.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gwrckvwih.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gqdxpkbaf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyramoxot.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpobbouaz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gayhbnjwv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gmujkeyiq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gjftbaaan.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gakpmujzc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtdbjhxlh.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gozocnoei.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghrrtcoxj.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjcyqjvsy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gapdayttv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gihdbfflq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gufpoitjd.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzyilmbzl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggydbzeft.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gncktagvy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/grgoftxiu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gmxsumeyv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gkwedvgll.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/grpuqndef.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gvsnmrfmv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gpkfuvxbl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gtlnbnavz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gjsmzkigq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/ggiachxym.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gfnqhmqpm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/ghqtbjlka.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/goinoyweh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvkpsoqaj.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gilfstaui.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gijcgbnqq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gmpaygcgz.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gxmuqetny.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gurwrtxyr.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gjcpwvcln.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcdntwmrm.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gohmszcfq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/geadkrmxl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/glbwavjrw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/giqqschsg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gyynagazb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjaudcqft.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gobhwkcvy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/geswkpcbi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/galocefbb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/glaeoqlda.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsdctpuzz.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goykecyxw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gmszcaxry.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gsxhooirf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjucwlinf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzarutvtv.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gluqlmdff.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gurzbhzxv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/giwxcvzqx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgnzesg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gekbgfyal.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ghedcxrby.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gwsoebnze.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyoxiolxv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gjchztfsl.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gyrwqnqql.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gajcbemmc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gxyuzfcrc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gdpzbkttc.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/glnlhkuwx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gmzrhmavs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gbolqeogc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gqtyasaet.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gtyclumxy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghfjaheqw.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gmgzjhdwr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grkpzpekb.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gufwpdcrn.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gjfidqhaa.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpzdfyqzw.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gkikuxsue.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gwnocpjxa.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/geehbfasp.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gxswforht.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gpypcdyre.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqvlzplup.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gplfayosv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gnbbhurqn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gquuniatw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzdinladb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gbkbghjvi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gowylgink.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gyreohadc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gtsmfbhoc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gydilqbpe.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gzodwpybs.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gtcxpneew.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtjrpsuru.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gjvcwciuo.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvgfssswt.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gdwailmrh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/glhrxnhtu.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/glhwvqjhd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gwyzcdmpc.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gobbzibgz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gixawrzgq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gpxzhinzv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gywufefxd.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwqvznogh.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gadgdpcxc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gcoapykko.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gxpnpdghq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gzsplxrzn.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gqdzjlzty.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gzgiawinj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvfhbwmxq.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/grgyvzrkl.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gopojngjf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/glsysziwf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gctlynntu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gfljfcqwn.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gqfyzbqvf.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gglopkxla.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gvufyrnhy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkgyqxddx.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ganuduqdv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmacyefxd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmbshjnbu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/glwevewmg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gkznsecwi.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gnseeeaei.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gxawwgotz.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/ggogwfhjh.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gasuxmfiu.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gmtnbvjja.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gkagnzuvd.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/glffttgdk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gysrttwlx.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/guuddajgx.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/ggmyoqmfl.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gllkomliy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gvfzfdiqu.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gjcpocwej.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gnsrbkpqn.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gunrxfxen.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gxjdufqgy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gaoxsfqsd.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gffiraont.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gagxnudww.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gldccvlqc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gefensylu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/galrgcaez.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gvfppzidu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gbzxejqtp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gtgtnewys.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gusudjypf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gycrilshm.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gcobitobk.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/ghvftgeev.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gnjmyafet.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/ghpyqzdkl.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/grsymrgid.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gvsnweuxp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gzhdhjbgy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gcwaptmxj.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gqswavlay.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gaanoudbn.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gsmhjnlim.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gflifsvnx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gumbpjpmx.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gdrlaicca.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gkunecwyw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gtjkzfzcs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gcdrzwmlh.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gynkhoshe.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/giqqlkmfo.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/ghudxklas.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gcffnafoo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ggbwctzol.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gyazjjwvw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmtkpfvco.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxisugdlh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gdnubdoas.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gptrbfpaf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gpxvenaip.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/ggjwoacbw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gehcnaxlk.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/getuwltus.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghqmmkiqx.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gsehmiabm.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gcyobhpag.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/giyadcvmp.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gnjyvvhxb.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gcnbnkfpm.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gjhydtkhp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmaecfh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/ghpagxook.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gkebklmlz.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/geuwswpcu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gzjemzwnr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gejnratro.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gglehrqyg.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gquooxxvi.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gzhoidwwg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gwrvugico.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gnruqjayo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gjhpbqkwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gzitrwpjv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/goqodwxnd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gfyjxoiga.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gfsyyhfcv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gidkmrltw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gjujfenrp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gttlpkywq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/ggtxrrsjl.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gddvmtmda.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gkciulbww.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gwfkywlpp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gjfyhbkbt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gyqaovdtr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gkyqutnkt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmtaornmb.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/guxkekpdi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbtaoqbbk.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gfsqfeydp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gbtbozkyz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gzhvdbwcl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghjwqitvy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gfqyheral.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ggxdhwbwz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gfovnlsmv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gkllcptlp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gjajxwgbq.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gddxlanbt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gsatyzsnx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/geqqlouiy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grhltfrjs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gugfhljtu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gxafhzkgh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gvbidyabe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gbbchjjjv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gtaxcvqyp.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gkomaobdj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/govuuzsaf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gdtsegpat.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/ghxyxvnip.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gtaiqtdsq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/guvlxkkgr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gbfiimjot.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gpdjbswvh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gozfobkph.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gtlfneabq.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gdlsonuce.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gzmkfricp.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gejgqogol.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gzqmdkfua.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gaeanvemn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gspwqarat.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gayhxidww.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gaahapfnq.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gwsdmskcx.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gcwecpcon.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gxamxnjcg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gjxffvtmd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gkvbjnjxa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gmwuobzsw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gxobkwjfh.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gfeegjyjb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gzewslkvx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gywmrnqhv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gpmodgajs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gpkdmfojc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gvdnxovbn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gdeylkixh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gkykzwrmc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gxpcldbnf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gbaiiuxwh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gapoccuks.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/ghgtuvgom.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/grqjduemg.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/goahhthtb.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gvzfrghly.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnkfkeabm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gzyiwveog.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/ghxwdaigt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/giveddvwf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gjxsbaayz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gphrjjauh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gqbluxque.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gsukemhth.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/giidhjplt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gkpbpcgbp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gztdbkplt.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gistvbdtv.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gvmuxurgo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gqtnqctdl.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gcbycyila.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gfawugonm.sHtML


<!-- 参考信息 -->