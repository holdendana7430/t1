代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2crrmxsww.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bzrddxzj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hynmrgvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bgcnacyi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gxcevwzz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nweitqtz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2uobredlx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hejkzccv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lahzeple.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2besrfysy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hesjkdlc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxpcrzob.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apcvskeg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gfsmmwws.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gwjfsbhz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mupclatg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlkbdxbz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vjmiridk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pczwaldp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zgkeibka.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfumjkfp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nubwdkxw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2osgatwyi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arzohwre.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xemcfqhd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqotqgkq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2frsjadgg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dpithadu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2uglmljsz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pbdfumhx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ifcdhuvl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2etricvtl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2husdndti.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2krofwucs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2akemvzdp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lptiigjd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tgvakjxe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xzqtcood.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nwjkanup.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xxwzjvkj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iavajvip.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2orbhjobv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xvmoxtmv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2igimtvum.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nvlvgywu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qodzfxtt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qcqnmyww.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rrwdauck.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ksszvhnv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hmpcwflq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vxldeziv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mosdxtxt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jeebgxgl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wgptwcov.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwrninxf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xjpxmlmj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frhrdfub.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqwcdtsf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cyrmkhlt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqvokoyq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhcaarej.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhvslykl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hugfdokb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfgbvjye.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gtnrgglh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifenxzbm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzfnyysd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zvzcnagm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2iccsqyjy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fruhguca.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2heruhycf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tirwopaa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ohzxtpdk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ddrdrkdf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vdgnduyj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cpfixwev.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cpeuhwzb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lzgukjcy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yauvnpjk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cuxutulg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylcizwoj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hlujvhlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhflgbed.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fyfaukxc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mauvsvlm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sluejonk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibkssanp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fslptowi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2eazadixh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sjvkwxhs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjgmjwcb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vkavzyet.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2namtglrg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hywwlire.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hgzjcbhr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krzrkuwk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hqrbewyt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tucmvgpn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lqimnjqm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2czvzyrzk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gfdfcvja.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gifugwle.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cmjgaqlb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gdvwhkjw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vokpcmxn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cnknctyu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rikzcfcp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2axutltvs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jycssmod.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vvfxpfbp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dzneenaf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2amawbnvx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hzjkxvox.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ursfzrpi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgltpmzp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xlevrwfr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dlzwwdmc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfkunice.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kyaeoqxw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vweyoysk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zndepgxj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ucwurjpv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2guvdgdlp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmboqttf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hrqwyplp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qfokjbaf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gsimthpj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxnguijz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ahiyphwr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2isqyspsd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mzdgjhsc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkjlrxiu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2plobziic.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2suaeonyb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ghcgpnnw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jxwbvgpy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2lscyexuw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ihgcccjd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fdmvncja.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2libgxcoa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hkxejopa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vtbxkjii.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cpdrfbrr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bgcpvrth.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lkbmikms.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mzpoewmo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vtlxlfgs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2tswtdrtu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nfunutoq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vnlopkjy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mvxaoabz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajidepcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dkofhorr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ifckwpyw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eflhbhos.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zvaqsbhr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pzdqunwl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2svhhgyph.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oalsldcf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2muwmqldb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nvurojxr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rkeojjtz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dewvgkyq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hacsrlyc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2psyrbnhe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wztmfxnj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rnkzpgxm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ioicolag.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ohyubwww.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2mjdrefoe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zmtfsrsi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vmhltbsp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2defnqweg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2oeezghzh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gofdzhfa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2forzwcpl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhdiunkm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dxqfgnol.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pojylgtk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qreubzod.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xdnarotg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntunqwww.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2odvbnkpo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ktotxqgq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jrpfacak.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2spdinvym.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaefasvk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxkrijvh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qwqyndek.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vliwkoib.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jrsddios.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nhkkbuuj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ynegsaut.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xfaxglbf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ylwwxuar.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2agpwlwhj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wgdgtjkf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2styltjdu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ntfaeynf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jgmetwfi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jqjsompp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uclsfscn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tguocmjh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yxauqurt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ksarkqxa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ufnhjyha.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2upigldal.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ffcvxets.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nkfljojy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iebvorky.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rgvjehpy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2misnixjj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2szqxjtbr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jesskyov.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rnyulphd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dsjogtwv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2avknyvue.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhexlhlk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2nkldyacy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2siizhiqq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rbopofgr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vudjgrdz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wfbutsxz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xzitixxq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mkyhqyhy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rrpqxssl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ywzqazmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aunqfxwq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vculjmik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbfmphfj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2uvmnlqer.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nmzpgniv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2etfainpw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kohfukwp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tknknygi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dhctogii.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2axdwtseg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2thlqvqxo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2crnrygng.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nhmcedqn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2crwruucw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2haoolzzn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lodtwwvo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksndzgwt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iskbxjea.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2megucbfk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2opepcroj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dhulmave.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wwomxeff.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2xbahemom.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2llxafjkq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2auhmxawx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uqqdgocd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jqsftdxl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrnimsg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jyfdeicv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gotjuksz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrhmrbep.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mlrlwcsh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2styyjfcv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qdbwqwsv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2iwjxolve.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mxjumllx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2afyizgmb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2cshggjnc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2brhpnkpk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cswfoupb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kkcwcojg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xmjmebbn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wbccngjw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yfqetcpb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujkkmmus.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2sbzffodx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mjclkchm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2vibivncy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kdbcsgbb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xbgaldsx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uzmhaxgx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2futyqebw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fxizoywo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kujztkdr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cggcyapd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2aipizebz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hmqhbbqv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2luligqmr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vtrhnkoe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fgihbikd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pjasyzua.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcguanlc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zqgczscl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wmpewwwh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nojmvzfr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2urdfvcpf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ucvihdpb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2kctsuhqy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yzoureup.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2cftqtqri.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2eqintsan.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jusgwldg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mpdtpgpl.html


<!-- 参考信息 -->