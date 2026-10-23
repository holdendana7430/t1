代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhnlnqrn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cilihgjb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dokqlxpo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3leyipiip.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckpxdydv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3olunfffa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqvtkvsf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mnbgfwcq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzqryska.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sraxsbic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hbhyezvp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tglmzvtc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfnrbhpi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xlrnzlli.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vkiraquu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3oglsutzc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bxqkkxyg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kovdppcf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rqaajgmv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xkrjmsko.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3skeytfov.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3swqhekbe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hpqxknyk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vdvxksjq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxxxahsf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lmotkxth.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tzpwymgl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3omatbnrk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pqnkndws.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jkybbtnx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3voaxkrtk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3momzwnkz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vuwobwdl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxauugwe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bykbrcot.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3onjehezo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zigmsveg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qmjvwepz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3iakgjtda.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmejtuie.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qaremulv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3kfijdosc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgaoxdbc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yakavoks.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3weaokrxu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfgwlkgg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jkknkzki.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icdcbsgh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npubezwc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nsavjirj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xpgtkzmr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhgoszyp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ndxzyjxv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsneabeu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtsfwmhg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bbmdthuw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cdbipqfl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zndwwelp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3owbbnydt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ykdnipqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hswszvmn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qgmjqwfr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vyjtvigl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pjifcsho.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3tvgzmeqt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3gwbcsshq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ocllqpch.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kijgensg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbohazqk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3skstmwvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjqtunal.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lipdqrux.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3opifftxl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfjtwppk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3enyhjnss.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wswwqrnf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lxzxnqob.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vqwauuen.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jxtpojer.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3goeibali.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3opefvioe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xiucjomi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3apcepwuz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nycljywq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rsonpxvf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhizfbrn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jqtqhuva.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3drmiyfko.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yndmqwlj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hetqoklq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fthgqgjk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hwdvznkz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bomwrnbj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bjjclcce.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dxukkjnb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cuhkgqkl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3idafbbhc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ifdahycr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xosyvvxy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fgpadmkg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cvquwzdd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ccyslysu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oihpyfje.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcbpcavh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mlbpvikq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3utqtdbsd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3poqqugog.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lvyimqli.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3eaynnbbq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbuszami.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijzpxzbk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3boaaobta.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ftdcxwve.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3njpgqzze.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rawjvcwx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3whjkbnog.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3usroojum.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dvarfuec.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlrauenn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nhaqowdc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkalgjwq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvkjicef.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ymqpgacs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpwkvufz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uoiynvfm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kpizznyg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wtgfjaut.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tgyvhcpf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rzsboyft.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pxcyxszs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fndigofk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uapmaepn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qcdmqmcn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rvegmvkf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3uhkrkcoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jlsctybt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fbgtsrmf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqwdaubc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdpefvjc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3exftewrt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dmnhlupa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tgqncfxh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vryfulvy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3chsilaay.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3osulnnmn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zjtaqedv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qqghhgly.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3llbmnwyi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fytxgwxz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nhztimmp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tvqvylwb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3muuaiysy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rqvjqwmg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vbrbydwk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jdcagzbj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jvidrmuh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rqodobaq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wqypxvwo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3uqswutxe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pganlnfw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kkqhtmdm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mnqdjawi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rpxnaomn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3elnmhoqx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qqxzeyuj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lymqevfu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gnbieuxj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ntepowuc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xfvcpjgk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgyfrkwc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wcdwgegv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qakznkiu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bspxgwui.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3onzgzchv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jcnsxqce.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cwqkzydg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pbtlernw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mbycdcqf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oksaejah.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cmydlqrl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wlykfgpo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zzgavxqk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cnggwfjh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xidviuxg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iuvswrzu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3quitbide.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jhcnweyd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wxhjmivp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nrmsjgdl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yixitkha.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fvbnsvah.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ipqenxae.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ebxirpzx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyxvlrsq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nwudnkax.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dihljdlw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xyiobrki.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xyuculdj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ucdrvtcj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xdmrcids.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3klyrnyaw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ldietnbc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rtnzxlgd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3brtdvokc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wicjppbf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lzcetwqf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3brwegqqu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rdapoqgv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rlvgcggr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hglgesmv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gztgrprt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rywtlpxw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3deucylpo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wvylndib.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gknnmepz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avqwxneg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3glpxcpvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsczmtwd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3airvqjkk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqiclbx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3enutezrv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3syuqijsr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uundnnuk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuknedrb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jmriaqiq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyqebmhg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3idlgwwuv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ztcsleii.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kufwsmzp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbygzevh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fnmugypt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zcrfrbhj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jenqlbib.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zfysaehb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnmbvlgy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxpukwsj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3bdkgssem.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cjxocdhs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xgihuhfz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cpsnvibk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eoivymvk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ygewnbqi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wkskdtku.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3azwaamqb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3atfmiyaf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3sdimhghk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lvltthtf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mxvfkwba.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fngphknj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rwiwuzmp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vafrtzcq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3yfbntqyy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbzskmrf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jvsnhaaf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3lwhkhiel.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3hdtkgjwh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kdondbnt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swplkpgi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfzbdaym.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fisynxvn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dnnnulqe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3oxxjiidn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3twubapwi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3mutapegl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3brehdjgn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eepcbmmz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pmxztgpj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xynxjjyn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3aalcfkgp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hsiwputj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jiomuyhg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rfcqmqjw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ilceebkl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ikpwelqm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3grmtgpfh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tehxwgea.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vbktvfcq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pvayzinv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3armzsknb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3tpgjabsf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tbjuyajz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wqcqxjnu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3momfsycs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fjkferdb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3jygagpab.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qarrcnlj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dxmwnsad.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rjaniqtv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3jzulvppg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ortrqudx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fvtyadsi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wjtykvkd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3welfpaun.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3pcnjdcmd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3yevwgbpm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkypbolb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3yxihoovn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qeawzgfs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3luphqylq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wmdxvseh.html


<!-- 参考信息 -->