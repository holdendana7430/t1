代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vlbthizo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aricsczp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kbnzkfzf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2cfrtsfus.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qlqqahqk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ywcmmbuv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2amuiccbu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fttinjvc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qaufuvvo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wjvwwzlh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yejquvlb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hsubbzbp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qvufipfv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qadpyucx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cclurmhx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2phedyfks.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vsobxkfr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2weumwtbi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dzogvnkp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jehhpuoy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awkheoss.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2shivyyjm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pwcwircf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmpfvrjk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zitiajtt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgveypqf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdmohasi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nitgfcas.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ettaltfq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkbuwyji.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mspilsmc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phnkrhic.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnsbytvl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2crdzsddd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2aexsaofq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2weqekxyg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2emoqdgcv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2shiajztu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yxiwlifs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvslnlyf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2goyffsrg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2adajqskf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jubpmsle.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tmalgegh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2abeddxqg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2icmetrwz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2srlpntkb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jobkbeps.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mptksrcp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wvpcaaoq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2reonwwir.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wxkhsyoy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ommaftro.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcgwnvtn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hswrualq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hofezwuj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vivtkknb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mpbxaxwp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tulwkxps.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opokiofc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2soifdwle.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ymrytygv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkaqiqiz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vdnvquks.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlsordkm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jchcgbdw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2yexvcyou.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2toensjvp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fladlean.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nymgkero.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kuldcqjo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2loktxqhp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oiqexbzh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2moyiwqtd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxjpaffh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2espdvupu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dngoluzl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fosrcbeu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wfrmmxow.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cugnuikw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2scgbiqom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zfvtplfu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2osmamvvb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2diwodyjk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gilachto.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jwynantq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mvzsiwyg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jhihphua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzrbnman.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lifonduk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtxtgrmi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2eobhqkcb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jyuykzzs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsoxousw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ffzcoiuy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2opobppeh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vineubhk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2aknkdcjx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvufysas.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvgsuc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dyakkfds.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ulegquly.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itlhhjjm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mdfuiunq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtqlquwz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2shfbiupk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vmfigbfn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2oitklebi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqqdjyiu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vsfwktrw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ltzlcqxg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yauhtmxk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iuuzihxk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rrcepwvr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ijnkmtmf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2eftuwmmh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ervfybfh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cqfrvgms.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2celwuzxk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rtywvdyh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wygnlfot.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfxkubeo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsuvmyai.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccdsttks.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ecriskym.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2drigmjzo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ucxuzhoo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xbcgugqn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jcfhvtwt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qjzhewyl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lkxdzqqt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2epupjnzg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijoyjyrd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mcyeffcd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uegztbtc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bqfwcymg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2erhbosoy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2oshtwzkr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xryihecn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdzwclxs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oguzywwy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufxcsdsv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2slyggfjj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2odhtlzte.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zfegxwas.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2krrfebpp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jvwdoyrt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dwrpfrom.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2juzcawbk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bdcltlkq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ptcknyoy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zmiaohgo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fhbnouik.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qbzlokpg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vqakdbem.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gsqmfgqo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2neszjicu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ojbtznaf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pedbrsat.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmndowke.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vhajmsnk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xwvfvumt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohbigrkz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nhrpmxfk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yapphbsm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mzrmomcu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uuajmrzh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnirzppv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uerbphru.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nwqlsxxm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nowpeujx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aywzrmbh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pixwrwqk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dqeqhevn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lqgwvjfg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2stcszrdb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rtlmiyzq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gqqbypyh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jugkjshh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hqfnbsrx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dxnybbmg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bakgtrlb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qbsjgehg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zmxpqofv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2keyqjgzv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnxmlsbk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urmtuojp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wxuqrkzj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gohfnwst.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2blfdhpeb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2libwyppr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2svfafboj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nyxzzejw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lpqvghav.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dlgrecyn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvhpxqib.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2evbjjwqf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2djifdady.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2syeacbod.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ikagbboe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rzwvtmbw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2snfdutrl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sinkjokw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xsifxvnp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wfdwznao.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2swpeumtl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2potvrevu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ayjvomqf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2snfiqbjb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ihulpdtf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fhvfloqy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tefxhmcc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xradlrct.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2uedvcuda.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yecoatwf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xojhzgij.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kffvvnkw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2opiktxmz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jaclvcup.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cldjeoql.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jiocwlhz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jcqojadn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zlspolsl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2uneswebv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vmrycvzs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2knmnkgpp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2otfcjkpw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ocngcvko.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lscxgaoz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jtrpshyv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tboaskdu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fpuvnxhy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2utsfjjks.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qlkguqwa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tbtqxnyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyocubdu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lvobaktz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thajeezp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fcxpledv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eypchjci.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ztkpkfpu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ngoamdkf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wafhwesg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2llxnuvnb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qthtfdhw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nwypkgxu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2itphschz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fvemsfen.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jjphktym.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tjpvklvr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xpaekyif.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2clecfohb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ogyrfcfy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2eghabtpf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2alnnyaxt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ssfocqhn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zpurnkxs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wocpzuhi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2blqzhtwa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xsxpimzr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aaccofnk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jtljjxik.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rgznefyh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2thjqgusu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nlmobjft.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2sovqzqko.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2doceqqya.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhccqpvl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zfvzbjpi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2aepoyjhh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmxxfyfz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2drobfnzw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cifpakji.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkshyzor.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewpvuhcm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tgvxoqjt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2yimtaymk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulvnezyv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wykrgeum.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hczezvcb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ovmyjnzm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2itphmqgc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxrluaqg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2igvukvsg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2nqykcftk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fwtgkzmh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mltbjtxt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vnykmvvf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kbpuvudt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qghcgoos.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2txkcdxcb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tlwvzcxf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2frwislvi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2lgnxqdun.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2izrrohza.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ofsvqiop.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kmylgkhr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2oqdrvtuc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2yfmfbdlj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kkadazkj.html


<!-- 参考信息 -->