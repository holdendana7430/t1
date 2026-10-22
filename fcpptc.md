代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnsomfmu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qozkgypc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vglsltyp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plmcwjtz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oacmqvdn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbybfixu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhidwxqa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ifkjkodm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2neqzacbr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtvzpqcc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2crbtqzgs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwbnmzhe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbsztkpb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hanevnav.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sjswflch.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mozdqtdr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2weshxfws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lmmlixio.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yhmtkuxf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2iictlxtf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zlcwerjz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jwsddupm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lepupygv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2aawalrjj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwwljbt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jhbcsgme.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2olyxswss.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rmqukkmf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eyopvsev.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mojlyypm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ieuxailb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gamlpeqd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ygkvmdwx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpnhpsuq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vqudcsfd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qxlvpgcz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dwfiiyfc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2psgeofrv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2srxmwidq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qyqbzwhd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tvijzozv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hohplchz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyhsialm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2okowdkmx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqbbqvaz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hltbglal.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fhwlhqxq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ropboopr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckfhpwkr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snptgyie.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvpisctn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tldtanno.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkawxcnr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngfoemwb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfmdcfiy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aveklwkr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2npfkxwkw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwsmbqzm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hqtpjzru.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kaqqpcqs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2aadxcykb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2oniekafv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2janrnzzz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fnlidbcq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gogmgwfz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ktqmcgpk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ameehczn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2paepmgrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xakwdcta.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wzrsgmqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgczbhbc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2igpkpvbr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2znykkbru.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hajfgfse.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dnzxuzhp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjikrplk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojydsrim.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uwpjienz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gutdzdny.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rdqvcxlx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2damizvpg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pswcztsa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvuzhrqw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbbydchm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvmrrzyr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebjcdklu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2erdugyvx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2sikwixyi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcpvuewj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hnzuxjbq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nrxbexdy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nfvteill.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qlsxlvvg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hxhbylis.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zhcbbsba.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cbmmxglr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qoifovkw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fbohhwmz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2idsqpycr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xfaxpqoh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vubjtpyn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxrjyxmv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfmhtrwm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qadkphnk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2buzofltu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2unqltuce.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sqgzenku.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lkcwwcwr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kagssigo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcyonkfs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kdtdyvit.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzanbmng.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydqzlrot.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uswxnnln.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nrstknbw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rmzmswag.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tdylljyz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2amxkjkvi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxthashp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swruhevk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbtiwrhn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oaqeilor.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dyuihhdd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xkwpyuao.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jyxobhmf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ueciqjsy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xvodmqcj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kjuidzmw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qleawhdq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vmdqhvtw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bihjvuqq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gaklnxkt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qnnohhkk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2fdtfvpcc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dwmbbltf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bdlxbaxv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2yhbrbpsj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpoykbpm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjirbkqg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jukgvhzv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2adxokeqe.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vvwotdyl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2duijxhmd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wqdnkcvc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qlsjynzh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2svevdwov.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tqylemkh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yohyskwo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wkuhvyli.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2jbaavwzo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kqewetzn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcahcwuk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2payzzjhc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dsiyxuzw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2erhafgkp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hekufthf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2msfczcpw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jhoiqyns.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2tyvllvqm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2otxkvqgc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fzzxoiyk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sfeguufi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bxcfwqre.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhnmopid.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjntsoxl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lhniiobt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zfjcwozy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mqhauxbs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rvxqdzny.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjihvkfd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cyyuqagy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2spmrslqh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fobzgagp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lozbexja.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2toedglff.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rlqmbpzz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pjnqlufc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pqfufkfs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kmgfrcpw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tifncgem.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dfvksxwt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xzbzeavd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mcxdpjmw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zynntpvz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2euisstwe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dilyeixe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2blamlscb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2erepbunk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2icsjpogw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cgmwmyem.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wbbqqapq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2btmfgtpf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gqvwjvus.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwajpond.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2myrqrxii.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2obrakomc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gmjqbghc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vldqpksr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iukhrsvw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2myinkzzu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ffdbmlbt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2alyszppp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fvbeucnr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rlvcpqwb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cfywiglt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qstgaiqi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2evhcgsmd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rcjvyxmi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2avhcteaf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ynqkhpef.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aysrispl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ivzuukmo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ctzddovd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jjsnlekd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qoanivnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2konipczk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jopsgrrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehttwgiu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tyztclry.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xouevtvs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bhmwcyls.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lcgbauts.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hirekypr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2kmdhbdlc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tarnilnq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2crnbnjqy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dynhzzzf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vigvdzyo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jtkrsvil.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2worazyci.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsefhjrd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtdndewp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnufnbfl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2iwztmnhm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2twyditqu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nrbcrgfv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xqcqofui.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pqomzxtw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qocwizcj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qijqzbvo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rmmzlmea.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fzrjjhoj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ruveidro.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2dcqujopk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kblttrlv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2akswwhgu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2exgpzviw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qhudprxf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbxnszrg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dktkewdn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mqvdjywg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2dxcdhlsf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2oruaurbv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovkduoqk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wtioifwk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pcszkjeu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ufokselr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edgnnoqj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xxcvwvwb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ypbtauaf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vdhycsyy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cohjcsri.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbgwjroo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2krojtapu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qrcmnpdt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yomidckv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2btsylohd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kefoyfbs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdnaqlt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tznpfddj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tzbkcyhm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xnunzpvv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2gurycgdc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2kiaqirye.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yftfmzqo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qbmoxmfx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xuzhmdzb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tlbevhle.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mnfuttmj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2txwrczyj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vyykorxo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2listdecc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hnvnexgd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kcpvfdbw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cedgwxix.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kbykfgaa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2maaswpgu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rorweste.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2uostbuvr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xsqyxkoy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hjnokosr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ikrwvgcz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2vbixmyxj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2jieoxsqp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yxrwzpra.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2mjexxzjd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2prsvoidl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bxrltsll.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2sqsuojta.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2upcbgimv.html


<!-- 参考信息 -->