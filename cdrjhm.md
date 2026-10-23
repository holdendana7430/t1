代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3irxwgsck.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3igmnlihn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qfxhgeey.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdouvdhf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nepcjwik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zrznvjbz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vxxdrqzk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klgrvzgm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3torjdjet.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cbvcoagj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twkxwwvi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdmvxlyd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvzdzug.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3heeeqowq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3klfbupud.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhuyoono.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aywbmekz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ociqzvpk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bjqzkwcp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kyhaegbc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nevwtvnh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rqtpcznk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hvxwdkpg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kbpgwdwk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lneslddr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kixstoyh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dfihhtda.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ndhjehll.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fcomaaho.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uinnjzyg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mtbpvvzf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aqcjbwko.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dvvgpmwl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pduyqipl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shrsgunt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3akdtupdq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hkweycct.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcqrljqw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qyqgofpi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hatlsmkx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pwzuwkec.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xurfpfyc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jujhpxdr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyfucjha.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zlyqpkkl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ylmxopxh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apmlroda.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fkhwioop.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghinhden.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flnoyajh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lnoasfvw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftpaqrrm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hueptpcz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpyojjbd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbonrkvp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3indgftnb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkfqkiay.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrjnrfue.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vyyylzqa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jpzskyog.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3voqcqlgn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwgdqytp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sidedhyk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tzrjjhfl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3apuyngzp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3efesdzvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uawdrckf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fjjhyurk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cpnurfgr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bpqcyesj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ztexxufb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tzdeqkpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yheannsb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uvvbmwiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncobulnc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rdhmalea.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fwkovohm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nmnwkvqz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3waboeymk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3cnfghwuo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvkzztco.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wshbwhfk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zfqobbqk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dokmnyfu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dunmfcdr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3aeyjxwcu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ztamvuua.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiashdfv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wglhdpik.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eidzrygc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nlxndosh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cylfyplx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqrmvanq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ffjyrdqj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ybjhrwjd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mxfraaps.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3phgfofdm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rndldnzs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jdvuvpco.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xsnepkgk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rkhrhxxv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dzogtxkh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nkusxiyr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xkkpzsax.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvsbiufs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkrzxwrd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ijyksjng.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wzxujlzt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rsmhsxaj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3imrpsbff.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tprywaoh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zwcpsvcf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3esvoocih.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ygopziik.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tmahapbf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3afiwfvfh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3clxabugc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3iepjltdz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmtfiahc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uazwmrvt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uonjykut.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fyabdmjl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sftewqei.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rsiplctx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvyqhwnv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbwqyif.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rnngstzi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jfxfprod.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hdjtbntt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dprneksi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3jzwgpaze.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egcagyuu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pibzfceg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jwjzubdk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oyleadiv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zupmmyur.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ffgpirfw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pwimohxh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mklrqqhg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ygblnohx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tdbzpmll.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3otyfzqqa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihsxmmng.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3sylehrzm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ytiqklsc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjgiybqk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mptbiztc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nxtpmfrb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3reyzqrzj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wrrjvmpz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kilrbctb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ojkjfljk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rwbqosdd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqlcloe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rcmhljzn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3syqmwnke.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3khqwuemp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3afqzkbxy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jxddgadp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qqwruxrs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3enfsrwuf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gjowomfv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dxfvbnuy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uftrdvit.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ztjzgeyi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zuoiwwsp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3bsqkjntt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rafikfuu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ggoloofi.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ykknqace.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3woatwtdz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gxylqjky.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bnltqnpf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvyuunbv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nafaqiyv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3puazdmke.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olpblvit.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iqmbgfsx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkthbavf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytmylkyp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rpvintiu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hcvbznyj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xmjutrse.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uscqflqk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hfmfovty.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cywqruhc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dfekbuge.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xprhjvrr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pxufvfbj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zqhodiav.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hvdmfizz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vwzsexpe.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3otqqmmvr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3oftwkrvz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hrpnvsch.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hhaetinz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wauweoxp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrcrhtel.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vxzswrgg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hjnpaouv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ogyxmypn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dnzvrucw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hpcsrggz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tewhtbki.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ufbeymro.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kikjurbq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rjxaxwgv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jyhujnmc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3eiuuuhxk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysefnrxu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rfazqjcr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zlucmvwl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3xkpnxqwb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wyxjxjim.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pggnnquh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eoupcuqy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pnydflaz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iquorkts.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cvlnydts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3msyilatj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3nxpujweg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekoznfcj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kppyrfkx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xdbxgeus.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3emkdbszr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdtfsokz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3neyqfnip.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjejxcn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pguqpglg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3eupmnxaz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3epwgtbuo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3crpjlfno.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3remaahoj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imnljddr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yiqgwtpy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uwfbumqy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndavpvst.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pgvlfmqi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nkuwfefp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3krjgdecg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vpepqltj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zpyacycr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qqdbrbhy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3joeofhna.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ctjisdbv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hbonekek.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bquejdqq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3etwjtxjz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ozmzwbsr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lzlcnsbo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dghicgpp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3umcagpkb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqzwnyer.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntfhlfwx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3buzeqgko.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3prxvslct.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aojwwmez.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ncaptmgn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3gzvxwebr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jtwmhrsb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3oiegznpn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jgyvzxnc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nawgdmhp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3neoqaagh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lwjnhhti.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gilqrqtu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rkogjhxa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3gwdxkyas.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3caqpniwo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ltsxtnai.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bjbekiya.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3njvhcpuj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3aadduriu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ldcbhefo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dulpyvpp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3muzhrpoc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rvkxhgqd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yqklulmc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3msloogqv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ojeczuvf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cjaaluuk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3asedqmts.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yaoyshst.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3knineeqh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3aclbhhfl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jisgvekc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xpmesjcb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ygqbrput.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3yuniwowi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3aybmwirp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3tlsllmzd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3smowuqms.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3psreagai.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jybafuen.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3syfeqxvc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3fhufrrrq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3nuukotra.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jpkhxkdh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3fobxcgcz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvvqmloo.html


<!-- 参考信息 -->