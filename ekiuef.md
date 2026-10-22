代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbclqnz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2llziygqx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hgzdkfyl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vzvzcdqc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ogvhklyl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lzfacael.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fhrclams.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qadhbfsr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scpqlrxp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kiyczhpj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zhiqadbr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uncgvswn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uowjjmil.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzdxktch.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlhzrntl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sglhulww.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipgusrkk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzcjzeqj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zbiexhuo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skaulrya.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cryfumgy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bqxabwgu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lfdallam.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vjbbgbqk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pfuemuht.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hizgrzlt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2siehdljq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wscpagel.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qqllwhkc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dvrtymhd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jrjhslkk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kbloesdh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2psfzutqn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xvjllklw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2squncgdw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2trylrpcf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2chjlmjsv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iljxizfc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lboqeoxs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ukwpjphg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rqczmwgv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2goozxasu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqbgbikh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jbctpkuc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vevnjalb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2szhfpcru.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bduqxeyp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gaeqztxd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lhmfqzyu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tcscuikl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sozeoxfg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tvxisnao.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yydlamaf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzyqnzzn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kphtfjuc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tttrqhmv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtvgkegc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbjupitd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqvvesbt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sauduqzx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bvdxveuu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khdxzwmp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqmpefmu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpsmdytd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pksdyglg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlrumggt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2boqnjluv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wtuyphbh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mjfxgwgo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bbgrhehv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wciimueb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2stogjsdu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yvuwlucq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qcxewvfv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qpfbirvg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ibxpgird.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbyrbdjr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kolzilwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bolzuhvm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jyecynhr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lujepror.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vhhiminw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnqtkdyz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2esqnqxsk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wzthoqol.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pnsjdcun.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rzptxude.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iaxeourl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cuchstjz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2otwpsgkh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ssyxbhgo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adsibnaq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rodryipa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pbchaqno.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xgkhmfdn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2passqrzl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qalpcjjf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fniemlih.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fmypyzqa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bvuicbdu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tacptvvg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2iisuxxhd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2guppjaef.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2odostlqo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2urneilkk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nrmyljjv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jzjtzret.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ovxiesem.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2njellxpq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gnvuzlxi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udpvwhkd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlmbuccq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vysorqpc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2econosci.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2niumhoia.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lqdnxzoi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zyqfxuny.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jarkywly.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rgmdkqpm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqjmnabc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vfywvjgy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dsaxceli.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yohxyexy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2otfgedfu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2znjqwlnm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2orrbyppn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfhsbtnj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwgvivk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kmxxelsv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2upescgns.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2njqdofiw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwhruhhk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nwdizfpw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vvgwbuas.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pildzfrh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qupldgyu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yyjxiimi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oautivod.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oayhcyfd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iqmhqfml.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mbdwsaum.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bmktafzv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dyakhtyg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ynqexoio.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2idejdrgw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfmevwwx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndgpwihk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2dmyjtexz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nwjwogac.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hjzzoxjh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lltwmmop.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qdboedgf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2utmjdldj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ocogkvzo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lfrhqnjp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdkvayro.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2piwpgbns.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pponhxjo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2chfodgdn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqwellcs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hccbapxm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jgexscts.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cuuoojdy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2grmrcwch.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qpemwnfr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fcxywgwa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tfpqgczb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jlcrifnk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zjagtbhw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ljyfbrrk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2duxqctse.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jqziyvxd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nfkxzitc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhgomenn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtjxlqct.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wcnrvnpl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ovdalwwl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ozebqycp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2icbrtwxr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sbbptwsz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytfrkged.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elpmyjbg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nwmtnjuf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwuqbxqm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nveyivqq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uxnlzqsa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hspdokzf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eeziqksw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rdhwjofp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qdyvdbuk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hwvcxygo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2efbfrvzy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2flajxivl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2sbcyalek.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kihzvvsl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kgwujmmz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lnqzfdad.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tgmovcsn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2byiewinx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2oelvetns.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cbnihbkp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwmyspec.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wccyigqr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ngcqvhka.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qyjldyux.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kqzgoftz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kbyryhwp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eywewbtx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rfqakdbo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2njkuzgfb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2nyvzusbd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2aibstowd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rzlshekt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lkgskmet.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xlccyayh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2grsenxij.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qyibudhu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ekicplqn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ajfbcmkq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pnsixatv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xpmhdpqz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2znxnlmpb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tusizhsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qniwngrc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2anzpfbkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ownzwtcv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xpmlpmqu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zjmeojwa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuryliqn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyvgmrjz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmmzbitn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2twczkwfp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ywffovgw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pykdnwnh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xsjspwyw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lceviumc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tommzetj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2arnoswyp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbmaaxju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uagnpbbw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lskwjcxq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2yeuyhrhc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufbxhfxo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gradcznn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zlxosadd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ruotduxp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2blvexamu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mcvkdska.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dgbcecaa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iivyhqgt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gafioqre.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bjnizede.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2suywzzdq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kdtgvyym.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rsscrllz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mwintkzz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyalybsv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kppgizuv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jxduajot.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pqbytosb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zchxekri.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dssmbqof.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kaskavon.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qvkayupn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xlqvsrps.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuiywyhd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axnczrwx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ksmyjiaz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hgexmomp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mbhxswco.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydnffamu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jvvrkexj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xbkjllce.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cpatnfwl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fanfwhnn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iahrnzgi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bfolsmua.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2qjjlpwkb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vkwiwgdc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mzjueifg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2baoafxfb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ltwqmnxv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oparabhl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vpreaafh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tbfiremh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2abiklrss.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2biydizft.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2phwagwgo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2feexxwvm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nfmiapcc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2udkdflar.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gpbqcuws.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qugowtkv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lbaflmdx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kpotyuio.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2dymvkovd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2iyqncgfu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2wtblhdja.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xerwjkem.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jfaphpmg.html


<!-- 参考信息 -->