代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cyhxyayk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pjtanzqp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dgcehost.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrelfwbc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zolzqenk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qywpxmpx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnjqcfr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvaullgv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgnmldyo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gqosklxi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ooxqlpod.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2swybdbzj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aonuklth.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkhfyltj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oyqxymdt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brispgub.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spgdkejc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2larhzheq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rfdxxuaz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bapwxewr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2emskxcgs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tjpqdonr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gugkjspy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uqxiogvu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dfavzogw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rrzssyua.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sjspskub.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2cbqradmq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gkzselec.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qgjtoydz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rdlzmcte.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fpyblqoh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sswbiyki.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fralmkmp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2khgichyx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lulekoxy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2deqtcegp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qkbzxpba.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ffotqrme.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dfgwdcec.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2puyajtwn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xkzwpinv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nkihjnom.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huioqwbs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jppldtko.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ujtdoiuv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojkhbkqp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2enjgahgz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulrxhybh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcjcbzfs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ccexusoh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2garzfrps.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgglzpia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slyetlvj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zggpdplm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwdyhuvy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxnokizv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwayktwd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfvdzazr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kbbqnsra.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2voqvmpvq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckrkcokv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wsdkypks.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kzhgafla.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ohjgozsk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xhqovyvc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jruagnay.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2civbjtsr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2psqnlkix.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nfyhacrd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mlvnvutl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uxiswasw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjdatxix.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qtikyfdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iixpalht.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tfyjbudb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jxyxyijy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mncxywjn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpwgiyrk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyyjuphn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2drgaqeup.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pnzmpvvi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bgdwlujo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdnlkfzm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdcftrxe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2suxgvlnn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmsynbog.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2urzztrnb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wpkkqfti.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hbdwciyv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxowqlu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ijguqrts.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jjxcoxdq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iariifwb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qbxyoqlo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ackkluuf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eitjyeia.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ixrjkyju.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xxwrkplf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cflzmouy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vhlasyxd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dftmudvs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zydmuqwh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nbfkayrn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbbydvbn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fowymkkh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yshnyqqb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arxhuyvo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yayycaxh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lbomazzm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uxcksvet.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2eqvdqfep.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ehoyyucd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjgnosbe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qgordhlj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2muibeuob.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yinbpass.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2nxgwqbsr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ontlakle.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eehuhbes.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pnnvwhma.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hbnujdje.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2alaisehv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzfmqsoq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rtrwoire.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccyobinn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rolfjbxj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2orjpvoff.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2julikweh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kqkwpjtz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2svjdppin.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wiprezqy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cqiuixxj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fibltbde.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jlewdsnd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2meaaoifo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bjeyocbb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ygxvqgnl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vwyptpxx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qvelwdsc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxpbpccu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghaqevez.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuytqfzg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qekafbun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dtyrlbcu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hgwujxzm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2byueaypz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2mzweycsu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jyotwazz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzsujccx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2betcdcis.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gajyvdjw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xygdvvrm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hhrcleun.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vtfrzszb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qjueqcck.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qwwhoktd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jcttofbk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vzcoqeor.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rqilugmh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vkozydti.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bmgmktcq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2iqzwhwot.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wpwexqof.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ettsubnx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bmjnhkcj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fgkylrds.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alwbkmum.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhdrkhbp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zmefukdq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukxfvfkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2enreench.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ftersooo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cufjtklf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fzcfxlqx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2erpvutyd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2prybfmgi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vezkpdev.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdgitvhk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ayooikdv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ghibyhyn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sdonshrt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lksqxhni.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ilivorua.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tomutaxo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2phpqnmst.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yvkekrib.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2koqhoelo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bzqoefim.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wsasxfwc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tofpopqf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2cahhpuri.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cnhwowbp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2syuhmvqt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dmbczmfb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jybbdtbq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2utrfwfsa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wibeodmm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wnnqjuzh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2adwkxibr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2cfwnaqvx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2azardwmx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xwoblfhf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcubzhpq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gnkqhquq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nubdglcw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yynqjups.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ocerjjay.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2useosdeo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2swcxvpuk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ltufqqju.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qpwwqaft.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2crrslmxy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jvynoseq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aavftjle.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zemxndvc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mhwailfn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2mfujabws.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qowcluau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbnyazsy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2iiidarwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojjiyboa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2clxmoshy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2amcalfwf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjwvrdpi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtmhdjs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jmeduijf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gciwxzpu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jofugjft.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vdniwvfj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2agbnymli.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ymytwhcz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2abynjpgp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wjpfmmxc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxtpaudn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mmcscteg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2opxirund.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qiqbbmhx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmjdolpf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fdsklwem.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fgzjdjbd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2oxlyqjix.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2avvahbac.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2patdjejx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jljamiqy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hxvwchqw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uzvpniuc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ipnahumk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gknaqzor.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gbdzhmxr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gnsmxnad.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ynwanoer.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubmeetqk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2anfftzzc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2eafpkmqd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rvdlidlq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bdmfnlul.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ybewsbml.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uxfnvvut.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yhtufqzc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2nhfwythd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yibcywvp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rfawxzxw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pqjfexdn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhwlgjr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uvfoukog.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlpadhyc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2elqjasls.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gfnehtxk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qycyvbyv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2shmgamxt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gbmcifvd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lmacqemw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xrydoinb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2irbjrhrk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2srsrkmhw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gyvthjps.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bylgypgv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ltwdkkmb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rmzwigqh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2prktocgg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2qiajiezc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2cqupbvmr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mqosdndl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2igjwgtox.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ndgbgnna.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2sczqwgxm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2swhqfraj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zppliqdy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2fqkwvkfb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fpxxtwey.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2dbmkyzsi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ytkzumtd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2fggnzmao.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2kkgrpqrx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bxusugzi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jophccih.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fsaurmsh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2iomyntch.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2leesczvc.html


<!-- 参考信息 -->