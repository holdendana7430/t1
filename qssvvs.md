代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cxnsnxug.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ojftjscp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hrwbucgf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3melrvpmz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eycwcxpf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3woprdpld.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dbcqndbj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwkxmymj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zoooxbxm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3sunfykrj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugtcyhvy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hycsfoyi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bimbcmol.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbggyacm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3odedggex.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jkfiauna.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfswgnnt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zcivlhuu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mpwhnplz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjzehrs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vyfdwjho.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3myzsvwgl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qfutbczd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3buqmdppm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gjiiqsyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ynsptjcn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vfygktbq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3apkalqot.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nmsamgkk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfsjtjzg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3chnynojk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ckoqgcjq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xwpqxddg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ejojkvtn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zaqigbsr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3orbwxxav.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ivxqfeya.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfschlrw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ulgtjxir.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fwuctvld.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3whatybvm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lkvuqmvl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jnvzmaun.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlmwcycm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3piublmen.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uovtsmyx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3msmbgihj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxsqqnjt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptsyactd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pkabrqqp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ghlazrsy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qoxakvpr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxfdgwyc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbkmmwur.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3umgtbxzs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moqbovnc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3izlyoecn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytxgwzuj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqqkbeun.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3blqueiix.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ygzaqmuu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3edofdsti.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3yfihewkp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kabstkdl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxpbfkl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qfjyhtlp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cepgkewy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bldlqrxa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pteikxnh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nwzfnoyc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dsjyjzak.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ylsrdknb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhihatyk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uazmcqdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwxreujs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3isrvvvzq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3egvrcgar.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bzzctqld.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imjanepq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbccxfwk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shpsxiuk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ezvtwfhr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmruzfjb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gfhgbsfh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3neinhfuf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qdvgjhbb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vcfkzyso.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qttmeutn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxdproca.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cutqzdzh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dtkzszvl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tzfwsqkd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lefojsbu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bzsvcyph.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3snmndnlj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3exzksfau.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uqthlmrl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uuojckuc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fyqcdbeh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkfytk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3olcnbjov.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bbsouiuo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3roziqzmq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iznxzzdg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fhekxobe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwzasrve.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sfvhxbdh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xijkjdmd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3szjfkqeg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sfcwyibc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jsksmald.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3mzgllyjz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dgzcaehj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cicoleup.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxosvedl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqqijltb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oabjpcsf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jlmvriyq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3btioercp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nltccnii.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3aqaktkqb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hagqmkqc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfbshvrw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxqcjoap.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ytvqykny.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oxwrsjee.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3iimjrimu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rgotbccw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bhgoroeu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ouhdmmdh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ynnanfgo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3nokczdpq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vsykuaim.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oooxbdtf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3goiezucl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nuxjptkl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3sfmvcdbr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jldhejia.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vbskvpnj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3otahfkej.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mibeezsq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhhpxflh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydajvgfo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oifspgtt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jplivpru.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbjvyxln.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tkwpxjnr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pamvpmdl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ubennkmj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3sepkfuub.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lootxmyi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zghahemk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xmmokcfr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3byogrcbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gyrnppxy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nmmddxlb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3bkilglcp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3utwieqoq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sqtueece.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ajnigdyc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uubrgmml.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hcgibjss.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3poxwosge.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yjxauncs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3itmzyhhw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3osewbcmw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3tdctpjsz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bhirppwx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejzmuftc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sqjwmdbv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecuzfnur.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nwzgvvko.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ywcoypqf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgskegiu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3sburzfuw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oreyonpz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zpmiowrc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onynetvz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swgrfith.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jorbwgcc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vzukemwj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3htmjjyqy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xcftywfl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vcosnpna.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3etrqeual.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3azzaoydg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3skghnbbc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mttlybsl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3meorddmr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3eivsgyzv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrgrglf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mzpapfcl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3giecvuiv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wosbnbyu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dihgvyaz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mmtvzuwb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3randzenb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3grfzgckh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oraihofk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kboieusa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hrcbojfs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uipzsdeb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3iumxlqsk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3yuwxbyjj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yjmdxcya.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ibiakrdv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3isnxxzag.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3cyfhpzsc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lgdlwlxj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3soplkpie.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3igblwcue.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3blzdnduy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3lpsiunhe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3drubmyro.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bhicgtjx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gklkvzpd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rxwpolst.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3otdfepxv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uptoejfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3riaikvld.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kqfxbouf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlhugxmf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rcdkywca.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3htpbpjhk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vbficbxr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dknwsxmd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpsiwojn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3seskiiri.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3frnoznvj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fvvdxqmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpbbqsxh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xaiyjgrb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zpfpscyb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrltoctc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nurfreud.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3djuenzjm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zxudygtg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pogrejfy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3eeoypuai.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovaejyzv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sobkstet.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3giaynkrm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nohaedrz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ylibirps.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pfuzbbxx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3agiocgzt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bxevztaa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3huudygan.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3divscheq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bpttzaeb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3jlbukavw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3chaibsll.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nagpnnwz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkwwwzip.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kzsioysr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kiuvzlns.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3imaddbhp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofagzctx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3savwhmmn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zpyjlciu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3krrfqcwp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxpzalrw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nfpbvuil.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppqgpjqi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xyhbtvtd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dbkfzawt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhjthnse.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jbgmgcxa.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3oeihunvn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vxkadvbp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vtpyelvf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xolcoeko.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3bzfhthsx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rduaiwjp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ohbpzsyk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qvpdjpas.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3pgiueniz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gtofokai.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ftdmrpep.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxivmbw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kshebdud.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yswyhkoz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ffrptjld.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3uarkcsrj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bxzkkhao.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ntdatxfu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hikdrgin.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3akznswcq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tillykwb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sabnpggv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gicgcueg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wqurfmbe.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3uaxsswdw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jbnrljaq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3qfykptyk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ngdgsvsz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3utbhatdk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jtbeuivt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3inysunvh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3emenfxke.html


<!-- 参考信息 -->