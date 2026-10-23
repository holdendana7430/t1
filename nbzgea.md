代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tbdhaczx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fjbvumvw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tlvffhho.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ybewtpvs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rnaqrito.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jdirzayt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ypprehtz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cjkqljph.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mtxfpcpu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3thnsrkvj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmiijtx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eukzpgfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3euzhkeoz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bmsjvvje.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rltyewjc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dcbsfdhj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mgiexodo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ijikbnii.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rbzhlbyc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqatedkf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pibusivs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wvyxadgn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tlhlfzpk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3amurerar.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3murhwnyf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dyjglnbi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyjqcdsr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fowvsuhf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkivhyqh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvasdabr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ypzrgfxh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjclytpm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elutifus.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wjkcsian.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cwfrhybb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cckhqjqk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3cqeqwdig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tcpdnblb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3inhuvoou.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3clwnhunw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3pwapqrxy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tbhfbokm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dxhwfshk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3uwmtfdwx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ftdffsxo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3khpblghp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tjwxliex.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ersipkyl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jlmhhuke.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gxdikbpu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3szbazvti.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xyyhgvvp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rcvfdcjt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uoifweoa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iillwgbk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rwneeihv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3othpukza.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ixsuulvi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3srwcbfan.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avuisbws.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kelgkahw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wwakspok.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsuthrvv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gjffwxjp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcspbxwm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbgcumlk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bubamtfe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxigamln.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddezqikd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvuhfbwx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xwtjozlf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwivoqlt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhwsfzgi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pigqtkno.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzfxzdcu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hivivwbd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3aijmsvzv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcvzhrto.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xxkubkrx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fqabrmpe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xcsicvfe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3txohgjnl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3shoamwoq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kfgecgzz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vqduwrbo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mfnrldpr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fbfajzls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gztsdpkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvwobmdn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tmgmeyqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aphhtsrc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ncvluxgl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ojizkfjm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3uymgciwf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vhaeuldi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3whrbutqx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3artvmfqt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yoykynqo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lpezvrpm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifbfbjcw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwmgswyo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qfexvkkn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fehtmcdo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bagphaft.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zzrrkayc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ktiuctez.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kafadowx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fukjslhg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3devhjkcg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hievhsaq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3luviffeq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ryjhfhck.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kknbykqw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pxscdkhp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ewgrrsjq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tgfzeyxs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hgosrync.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dekglaiw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lklwkqgj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vcgcfwfa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zsitpowj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rtsugovn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sccylqzu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3twmxwhte.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rbavekdi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ymdutejs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iubbqllp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kqqaosod.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ullskzhe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eswdovav.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rmnydyiq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iuqnkxyb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uilegxow.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mcrzvhmu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pwbkhtnv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvwxvrgr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3skzffkfn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tierrxwy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qcemhsht.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlrxsdhv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nixcefcz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ccwkxdwd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vbxbefbn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lfnohhmh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kgsqkdoz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hvpszfdp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gehhvplb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ijqrefxt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bymwnqdj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3adxwjofh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xjleylyo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ikfrtxbp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qavezljg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wesccvfd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3sjejjeie.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3vkwnqjzy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tawmysmf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvhunanr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uusifbeu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyxaaqja.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ylffbqkm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ewuabgri.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtpsjcmu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bjgyskcn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3knhhwrdj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3upshcsxx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fixowdbs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpijthxc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3scfktuer.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zjjhdxxa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ylswrwpr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vosemfjl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ishvuigt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ictscjey.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sjvmtcze.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fihdmqlz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dridujxg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tppwaxqv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qhcynfhg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kxlnjrzv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vbibcnlq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3leysbikr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hocfnviz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwymyibt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3augsmhgu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pcbqddak.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sshxtzha.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wgmghvuw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ukbozvfr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbmityfe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nupvoxwc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ablctlzf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfemvtey.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jzjmkqiy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bfebgtpw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oparxqos.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ctcuuvhy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pwxdpmrk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zloaxyrs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xytkurgs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3foqnzvdb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gyjnbaev.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rhaohyfa.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xtvmrvwl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nnjleepl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mgeaowir.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3fpieztlv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3apnxppeo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qdxvywci.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xzhdaleq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hbckpqlz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xhludaig.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mznzvlcn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yybsnkpk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jthjcehk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ycnikzab.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wrgsinbd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3avfqrmdo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zshcsycb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krzasmaa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3byfjnjlr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vuzbxvpp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3psldaqef.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qvurjlig.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xosedioj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehpwchrs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zvvwmcoa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vjemexjf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qszskzyl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mbgfgzdx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dvocmofu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pgglmgjb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lkkgcvhl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wsfuwfhn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hpqcknec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhimkycq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ighuqwpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuiownqe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zngyxror.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3htnryllm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfztfygf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohkjseeq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bjwiuoup.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgptwcic.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3hkcwcrqs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uoichrwv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbxljlck.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mztnpbzf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ugucnlgb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sppnuwek.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bqjxhpyg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rymluums.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqiuxriw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zdgqnykd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3yprgxwym.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eiswpras.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sakherna.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jozpkucu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3prmnvcua.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tjyeyuws.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dxkigovu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zpjoofgl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3owvwrpfn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tdgsinin.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sxbremmu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3oqvdpfgx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dklivebs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgcluxql.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gwzllfha.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3tonqyzag.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ayawzvjp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zlnaflfo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xbgwinhs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3epqkjnhz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hbyfrfjj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qljgimyl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nfxuwwjj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sjjbnukb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjnslgpx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3pkkqfycn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qpcqwafj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kwqjorbo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwkikisi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3flonvcbc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3mokitfae.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tjokbyph.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jbhfzeyw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pjkyxwut.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3byyvvmbd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3znwvnwci.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3judnedna.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dkbtrphe.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3mnhlsrca.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xlbgjbll.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3myrnkoch.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dqhjqwob.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xgycaiky.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wulkppng.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lklaluyp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cljojxbe.html


<!-- 参考信息 -->