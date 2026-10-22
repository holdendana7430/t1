代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jwzpxvre.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tyuuzkbu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ktreyher.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sovdqsvf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qeelwytt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vcrlwuna.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wvrupnig.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysagscyi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lagonyem.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2blmvfobr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjiddxet.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbzmrxmt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2diwgquuj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kudvfihx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zhomvveo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwavpem.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzkvpnjo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2edalddbt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gnkcadxj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2otqgvurv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wbxuevai.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jbnfoose.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sgepmjjp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdodbbnf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jubahtzf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qdezqngw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2isozfdhy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kjgbsxie.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rztwfzuv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgdcuizu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xjjdsrsg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lwwvwlfd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xqdyncar.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2twktebpj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fovbaumw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xqmbstjf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wotlmxlr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yiuuhoou.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zyoomezz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dgumltoc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nlyiizmd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddxmbtbq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uijzuhoq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irmnbiwu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ecwqjobs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2whxpuddl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fepygxic.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zpuczmcz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gslxdrzb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqkmkixp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tlvfitsy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pihavrcj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abwylbjq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2quhrusje.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vdyhcmap.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmsnvvhb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mubckkup.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aiwdexei.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqrytckv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nuomobmu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hqdfynca.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzmcjrgu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2eakzgovj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2taqexeja.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2niooibgk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rljedzei.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bnojtazz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gnwulyvv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2cipymlsu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2slpknppr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2quzhwruf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mhjdftcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zboymvdj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2aviejvbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okijkphc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2eqqsxqtk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tkezhfgv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ntrzghjm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpxvjbhv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mjbiatub.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2havabfmg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2eaccosiy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uoiwslmx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaqfhvdj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ihawkviu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2spijhtqx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2admmttyw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbryndnr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbgjlxiz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iusjzphf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jsqxlwyd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2woftrzzf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apwvmqwx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kfaztmqb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bklhiklw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zllphcxu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cztovcwo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dlgenztl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zuqmpkby.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ommuwlon.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ihjwrjla.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bfbmiqyt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xgfvjpwt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hwbohxbg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zuhwuqnl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hlenpuoz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2babmxlgl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hkvxlrui.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lqivltkn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qctafhvd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xihdphla.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rwtonhrw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jlahnjca.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2seovglgu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiohhkfw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vxpjwvit.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xdwkkrhq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2krvpczpt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wyvmldrq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnrhqbtv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dvmhmgrf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tjorpipc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2trblbdmi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvoiuhpo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2airxfwme.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nftpppfc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2modxmncy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dwglxebk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ifhcidys.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fwoxprkr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rqzokufs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uvvlipwp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2begsilaq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kedylrfs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rsziscrr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2huejjrtt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rmlnrkks.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cdasptnc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bnyicget.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gvwnmyfx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ysqfgenq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tovnvxbt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yorbeemb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2acnmtsay.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dfvtqchs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nxjljpnf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ffdxozbz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vwezgxjb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2blnukybh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2trohjmgz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qvdqbmih.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2pislxvvo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nieherew.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gsotwvfz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fqjpadyu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nqerphnx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fthngzgx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qwysboda.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jhzsavue.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2avcunhpj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jwixclvt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2btrccbjr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2okjrqvcs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hjhdlhtw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2yskqxhcc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dpeolcap.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2crjelpfd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahjzfzju.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbyjlmwf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2acuoszun.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jytslohp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mcbnhnen.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jcvwxkeu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gukgwttd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpnyoxna.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iujerkfy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkuixrap.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sexoxaci.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjkccwtd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oezltcud.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cztjdphu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2efthfujy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eaafsugr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2urrjuyrj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2eoizcvod.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fkceqqhj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ntulstel.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xanmtncm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uwfxezie.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2krlsiuib.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uphcgsym.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zezljtsz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gjxjhglb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qqtoecds.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tkqxgsxa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vnweooxu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2piqbxcvc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2slkqhlxr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zsduiamb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2juxebzxf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hugubeto.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2djkywrgr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2akmpzfah.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qisqfsco.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2iqdoyhpu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iavklxqi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2okenioup.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxwevxq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2obfqeapr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zgaprhuc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bjiphixk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nhkvznno.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2sbljrlaf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zmrwubkp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mrfhufca.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ezrilvdf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2diqnxfmj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zezexnfs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nicimjpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilwdprwh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2glghjyxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lynsuczr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kraxbiea.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2slxiconi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bxfngmtm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrihlxwi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2empzmbxw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qruevqeo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2miqiwjrh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwdguyvv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvltjkwu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gikvmhef.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fehchmol.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iootiolz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fhdnqjnc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eqsdrscn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nqtnlmtk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2gqxtggjk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hxiqxcvn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oomamkrz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mazepmtn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fgoujphd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vqvzltpt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jvlohyum.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ymaefrtb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rkwmiqzq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mijhfuyg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qfsvjmps.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vmwidwqp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ljvubjtg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tokutvaw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhgyyala.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uxnhvfqp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ydzlmryv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xqhkcykz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2iudhqslb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpwecdzm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmaszpmc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xqkwxppz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ogudysmu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2akhjxebt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sahivjyx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kbrodlaz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2sqyykzsc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tykqhwxf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2tqssmill.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2otvvhduq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gwgphjho.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2paedgbpk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vhiivklt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xmfeedrj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2stleamoc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wmbocebq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2egeqdjtg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnavbxe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rkhcwqcn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2bmikfavd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fnptqqei.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2whpjqwpk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2czrvugrm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fhsausna.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hjfwxbwx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zkqbdpft.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2aegjxpgv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rgdqscwb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2tihovqdv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mrddwvrq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2zmhblync.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ettlaqfr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2glwgnahz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2btqcrana.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2atwyvxnv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2otaoyclr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wfomtnrr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2apyyhnjy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gumebazf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fbpnoigm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vbzroqcx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2tauiramk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2znmvfjpv.html


<!-- 参考信息 -->