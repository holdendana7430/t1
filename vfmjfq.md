代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jnzydwah.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nscqveec.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gmfqrbfp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jtcwiwip.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rudtgnub.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jvfebmsg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3evbfrvoj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xmyxndti.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lzirbzpl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3amjvnlsw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pscajnzb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbftzbjj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqcftkau.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eskbwxhb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3whpmoqao.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttsnirxc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqpocynh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3foxtthit.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvzuvody.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cenqusjs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkrcbumb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afiqdrrb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3etwjbzdx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okcqtddm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmhcwkvi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ksciropf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3atamhjqd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mfsnnceh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mzhkxukt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3orbmvgbn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tonafhfg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3azpytapb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3oikghayg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ijlusrfp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hagqhfyj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3secohyiv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jcglggyo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvdaigji.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yrkprcwu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ydkfoglq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hvgwgems.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3moimkknt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gipuvadv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ezrafdtr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nlgsvzwj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjavhhmt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fmliiuhl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kynrcyci.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wdxnmudc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vajrayps.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bxatsqxz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkrzexiv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3odgdhmqu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jmoompfs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swyeydna.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvzaozfm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjtzzbdd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vlabovbf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ccbqssiw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3difdibeg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqzohlox.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzltvmzk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajwpkmwp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzampzae.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtmywtlm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbbpursu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hblpgwvi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pvueqtvk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zxrdbbuw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lezrqlku.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ddqhcvzy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wdadsudq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tvefqokh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3oxmeammh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3satnqbms.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ergyueql.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ebfhkeqb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kmvyqann.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3uhhzphis.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cqnizofg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edxfdrst.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3meiucxcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqiwndoc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rnmionfj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gyvaubxv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfaaxpig.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pnhtlbrs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppohecqq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cgslpyha.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sqsergbi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qcjhpllc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lerrxbpz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3thtsrwph.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ntdeffhc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbauawie.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3grkztfzb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwfbyenj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bjwbouzo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ddarzmsh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sbgsncge.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3goltutuk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3yjbocsgg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sdjvtuwq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tmykdnzk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mmggswja.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3pwrwptku.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qohwaoru.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wsjhgrxs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3umvedmfk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hjnnsfsf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3awidtsuk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vqhkfmev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dhshmejc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhuxcukg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgswrgxs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dblberrk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3esjvbkin.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rhsuwprf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ftxhbjos.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lmybdgnq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3scskrgwv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryuzbfin.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rtjgcmyj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aftswmyi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wnwofxbn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ctvtbqtl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yozwvznt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rgqlxnrv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bwmpqckq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wnophikk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwvmpbzs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ajywwvvv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3okqvjweo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yoemljcz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jaflsliw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xcsqfipg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tqsdzadi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rjrvdvqm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mgxcyhqq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kzrqowwh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cqgvwcpb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kdrtsfza.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ziypuwfs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gewjlzcr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dkeksnip.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cszmqrcj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qdjahxld.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fuejjgci.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ssqkhmyx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lshipkvd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgvuzxbk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kocbtusg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nptvmwyn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rezcvdna.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvtaffbq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lcmophhx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tnkzextc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pzlsocla.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zooclrbz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ekibfmma.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xbxtcdjm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ldzqzbgf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bppycaxg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aurjvnxh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ezrpyiye.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ahgtdvmf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gvoonrqb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3borbgpwy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vfaqikcj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rgsgjbyc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ssnfqlcn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bdiowawc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nibidrqf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3stxvdagr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zshpwnsb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqcidqjr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mumuxylw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtdfglyr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3efxmzden.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jdomahfb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mipxxavq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jcftodwz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3illahcvo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3idmyoayt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oblhsouq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnnezsrw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oewmlpnp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikoueumv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dwuxepnd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ywltoaxc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3olncofuj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3eyaoskkt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hezehnhb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3anrmoqay.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fqsqetqk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vxvibmig.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fiqiekxx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qvigkqzf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3juemhyhr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gzcbuwvk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lzcnnuzk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ydreipua.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tdthrpdh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nbsejksv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vygakwij.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bxemjdpz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ofvzeluf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3brvaoczq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ytfnmitg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qlnzbzbg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lasgdslh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3cufilcbr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hbuvujqx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hulsgumb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fybkvnwq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xhgooapu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ddgtjlzn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hnsctnys.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3umektxga.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3tdnvfhzo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3spoorrze.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jyepconc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tcxfviit.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wfuybrds.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3njhkpndp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rrtdwqfb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ywdrnbqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdhyqkpd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gqubcltr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwhltfzy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3whhpacbf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3orhtoydb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3itzxeljy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3srfpdjzp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wwcsmkiv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlpozueg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ycexyplg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3dixqynhx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vafzrefl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mqabqyqn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bxibxkfb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuqrxfth.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnuvij.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vbmumwpq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ayrplyft.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ocykotln.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ejcoeyqg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtiwcums.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ozjwuafe.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3brnqujpv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zccvejjm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kmfdqxli.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ngqvcglv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hydlgrvn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zfczlykw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pxaxxaqd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xbjizrqq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3nmmnxykz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rctmryfd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yqukjywa.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jhrtduai.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbciianp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hwdaascv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jisofojg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ykcgiedg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ymozvxtz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zayuhkrr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3uokiwrfe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3glopezig.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qabvbirv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bphlkhgw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmizktot.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nzdrtujl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3iyabragm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owxqfzug.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3emdjwcar.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3onabdtee.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3alzbdtcv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zrxsdtub.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mvnybtsa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vkydnklp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3upptiati.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlauele.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3brwmfltw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3venqwran.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wkdgbwkz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yrztlxmj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pfrisllu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zipotces.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ntgtbrxb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lbhtyeoa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ekdtdoti.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vwwnwlqw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dgdggujz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ndlbugas.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dyoegksh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xccgpiwb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uuipemmc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bumjfclb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bxklgtld.html


<!-- 参考信息 -->