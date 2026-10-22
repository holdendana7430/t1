代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iywntxvh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rcfvbgob.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2njjlqpgb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kiuzhbto.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpmaptsb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kdagbloi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aohvvsxy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tmufyrjs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvnrtarq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xytawbqt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jhwvcpyx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2prcqffdq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzztjhst.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyrczcim.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2agdddexx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nlcxuiam.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tvkrfuep.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cyvqvllu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uerkdnow.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rqedjaov.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2iwritmud.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gdmotszy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rfztwyof.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kjrpkysw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pncypfub.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kwnisirq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zuvwdbec.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2obuopemp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rsbhayde.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cygegvkf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hedfvydk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vvdnlrwf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lunaeznq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrrccnro.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ptpcgwqt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2witltjpb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kplvlubf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zeexlrpb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2emibsxds.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmtbayoq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2firyqqsc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jwhzwikn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xuwsczck.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmeluclt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fefteavp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgylnflr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kmmhcllr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2shrpidxt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2moziscyr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npfmyqmq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwlfsgcc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unydbnyd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zhmwgnov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntdgoqdj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vexnfvti.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwqabwvp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2eohfpove.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxppkydy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vqmkyjmn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2chnjvvlj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jctutaio.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hywonbpf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pdivjxwo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ketrcogp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2emyvvdgu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xcmemwzd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vjkwuiuo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fnfqqrww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ittigyoq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qqreizcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbrflrhi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kppjzyar.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fnhzfizy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qibmoukh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpabvpgi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zvuyghaw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tiuaerzr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kibqmmto.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fzhwsgcn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpfbpkun.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jkppkgxg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2inbqbgwc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmitavla.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2umlxqllk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jkxgkrvd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qsotniam.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lggykfrr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jevgxlzr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2olwrnrrs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zdobzxqk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fobbkwxr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2msbfutjb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rjtvsjtg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rvaknghb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ocxtmfrm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cdqjumyi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lvmsbjqn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2evnlchkf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ydxkbefw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fhoyigmx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cqnlmsru.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gqzhnrah.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ueammuux.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvxbcacr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oglqwvkm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bywhzeos.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dhreaoav.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gmjvuvxn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2oxiswgok.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mxlzxiwi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzxmvcmj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2flkwcjeq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mszmrzri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ljtjdxnz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2obzwsvlm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bebizpam.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hzfxozwr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hslxqnym.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwbgbdvt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtgzipvw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jaxsnhlf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aozmplwf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fqaysnma.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zwykpeqh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lodufkar.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rpokihfq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sjmudazr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rctuxclf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhovad.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ptlxcquo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xhqirpok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kteslpms.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hcyuvhbo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kxakdzdh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xxtxeozj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ldakksgq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ocgswwoi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2sfvgkkfx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvkwlrff.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjcpvmmc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2myhndfkm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yzarkmaa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2paptivkr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ytmywcch.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sqayxvqe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dmgaiqub.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2etwadqgu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejxeleva.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pleurpbx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2aiiydpje.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2teehecag.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zzwbeutq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2aokhumrb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gfazeauq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ivackzro.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ugrroyna.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2natavcjf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cgyieyae.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2myowyikp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dqlccgta.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2jhimzkbo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vmberhbm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ivpsntot.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kfnreymv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kbvdvxih.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2elvrpabh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mvietcoo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bphifxhg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2njjionqv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hfqjpsbf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rhbgqqhz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bvjgjtnt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqeskmkz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeyahwtp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eryctmhw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pkwgsool.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mpopuzhd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ohnfmovl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2swwwzlqv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vthccshu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vhoquvzg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ybnmpcer.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urgjcnhi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bizzzjsv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bhivmgit.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2adrdcykh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bpsrtvkv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tlgosgae.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2aooyaklv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bepmuwfd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kxejechz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2giowtagw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xmpjsozo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eausgohn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jnobhcqk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qjoliysx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ailgzizc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2otbalykd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvuwaonc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rpqyjjep.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2trckxqft.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yuzalwfi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2igedwzeb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lqvlyymu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jhzhdwlr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wjqqhvns.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2heedtopm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bnfpinyf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vtosjbnp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gpphgidk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zqozondn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mwgpjotr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gvtibxir.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xffirrqb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2unhaiklk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gexkjiqi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kralucsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofmnlgjl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dejfmidv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rfrcmjig.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vnamhsmh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fjiefwcp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iekjhgka.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nqdwyzkp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2uzudxeln.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xfqdgimp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmnpidge.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2czdtymqm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2scvppuxg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hecaoevv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cubyurwd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qijsdotb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpawjrvk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2scmabouv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mulpwbgt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hahobpcb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lvoyvcrh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ysysplpl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bwzpwrpl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uelatywy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wvkwxwqc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bkdpofdp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mzitspln.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bbzoebpe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2huypcpyy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cerkdycx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rrevwdng.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuuhqccj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bdarmgnw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rzdibqsq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2aftqtcek.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tbzutgux.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqbcvifq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2kidfblgi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tuvtbdyk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2smofutyc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2sfkvamfx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wqpkbnbq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qwfhrzqf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snkgbuma.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xhnofhgx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wckmbwtm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkohnnsb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vfraiptk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fhbmtqns.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kxnrekta.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mzmugkhk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lskkybyv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2levseohl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vthesiie.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ualqvnuj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xhatfbwe.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2stkfviyb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cgcrwnik.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tflmgptx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yxkjbhgv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2brymxmjf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gllyujxr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vqrdvcjl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2fanobofi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jxposwyl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xprzrqzl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cvugicfs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qxpglgex.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tohbspep.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2osdfhhdp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ajtoickn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ayppklcm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kyoaokjq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2osnrckmo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2lbkkmygb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kzqexice.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lmlfovhy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2pavitaxq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hoayuwoi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jubagktt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ixsapwvm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vcbvapmq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ikuvnlur.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ciflkdyc.html


<!-- 参考信息 -->