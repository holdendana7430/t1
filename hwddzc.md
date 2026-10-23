代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tppfwdgr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qgihioch.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ltrtmggc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjxtrhdk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ziqwxbbz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibiultek.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aozgypcv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zbhdnrfs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhqlyyzv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmnucfyz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pnfzcqyz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtnpfehg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnsxgvlg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qvcpefnz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yyfjhmpg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mmduxzgu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tcsgvqta.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3joqqfdmj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ksjwbuhc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ykqxbooz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ldmipudq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3eoosxiwy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3onviwkfs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3sniekldm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3slwqerho.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lublnmrw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ittrbsad.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yizrjhqf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lqszdehj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hqdiiopo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ydqkxqjl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3guwazagm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3owsekzlv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3llrywyzg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tdbvxzgy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jauldmpm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ysknisnm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qircwtzm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vtqiyjhf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emfgvoyo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3pvsknukw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bfhqiqck.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3judhsmuv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3unosnswj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rznvamxc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ostfdizm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3heverjsq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsoofsbb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxttcull.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ayheoddq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfezcrfd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjewglsl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3orsmwjju.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xopkwiej.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fsptznut.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3olufbnjw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3blimqanx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bczqoezf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uzkdpyno.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3shovpeed.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wycgdidi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3oygnuxxw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3eutggsbo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ljwzvvue.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mcmmvnwt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nhkyfavq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ysjkkicy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fcfizist.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzlrqhnc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ihugmzbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjcdfiox.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xadcczfn.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zothxxzi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3emelispy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dywruwzh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zpxbkkhm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxtseuss.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qsyhshlk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wdlefekz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3faxacrsa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pocxsuro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ouwgcefi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhmcvhal.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3thuqbbqx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pqypuqdn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcqhzbgh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3iyumxapo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsxkknvb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpkwykhg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mealowxl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sxziydlo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vagqxlgd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3abkrfzch.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bbjaqlwa.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3veafkliw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3psiyiwlb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jlqzxhnd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xzrxchgu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hbcxvepj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dhhmbwcf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ylunogld.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nfgrkaot.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ooggvmvy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcoekqbc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kwhinaav.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qtivnlpq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qcoiyaph.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rotosbhf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lyyseosk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vvpfxkvh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qvopfnmu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ugpnlrbl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fofczprv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gbchmwsh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qegjruuz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzqvrfve.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bugkavmv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pgcskhnx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lwgjxkyh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kfrledhh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyxafavu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3umbgiati.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ekceyyxx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tfvhlpsw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zkrspxzk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vbrazemk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3skihnwmz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ujbvmxbh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xqcggpdr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lioszhls.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uowabhsn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3upxmnapf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tpltopdv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kytyfryu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3utfgkqnz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lsgjbbfk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbpvqaus.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbfjhrdc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzqpqygf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3icsvurxi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fsfvanzo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3eisasqqa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3efdimsuh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xuswyxos.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gfvacsbd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3huunwnpo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3isavyyim.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xdqtbqtf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dobhxfra.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxzuegzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3khsajvof.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hgazwuex.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dbtcltmd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xhswqyas.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cgdblsdg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bivaeizo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ntigdzey.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3irhwhccd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ahvzcild.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hhyuqvlh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dfeewrjh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zmvozqrv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pnjazrni.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wdprzign.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayiiqwgv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lstmrvng.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpahdyyq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vdlwbexd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ppykbnyk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycgknsnl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3klzceqdx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qysryswg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xknwwphs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdzyvlrw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mirpnecj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aqzgwrkx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3embfehel.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3stcxctzk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zlyumlfq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nxayevpu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ugwqyair.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ynpltbdw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qpvdobgp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3reonivej.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pyhroauz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yidgpnqi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lwdldvug.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3donpgowb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3szwkrynx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gmgswvvw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zzlrqysk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rlbzwaun.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zxpftfng.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qictubof.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mvbfjsbs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3uqntcbgf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3uolwdkyg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mnspgcbx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qohkhxhe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3boogfczc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pnjasrlr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eoexpjmq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hgkgwfat.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gozptctz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dbiqcknh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ggarsqvd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wbzxemws.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jffxrxsg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wsckcbby.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvachfx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ktchgqxt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zlzkrzoa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wyaihfbo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ezucaqof.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qnephlhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eamviobk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kavhszjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzkyrdpw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3indopxck.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mshjadoy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxlmsgdm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fygfrlni.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qoehmgvj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxoenafw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vulvjmou.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lzqqhmru.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwjzgcfl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3esgzoazq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lekzmkwr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ndbpgaph.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kovwwkyg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lwxikwxz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3veepleuu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3aoknemvc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lmxrutaq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lyhgdpoh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xejuxzax.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ddbwslev.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bnbqoeav.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rjluimar.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eydoaqfs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbsvnjef.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nhlvsohl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qvpexdos.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ohhdzatq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ogegmoaz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3htcqxsnh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uaicwesy.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qgfumukb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3veatonbi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtvhrbgl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vfyfwmux.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvxyxbcm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxxkdggu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3szevckna.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hoxzvbqc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ltjzqntl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itiycngx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3epdlnuye.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3uwdnlwaj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xecdlwdo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bhebzzti.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmhzrneo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3kakxwuwu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vltcoppu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dxpnhdec.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fylcysbd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3maleovhf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhbhrgg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3uqbtzyap.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ebhbvyza.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3fktjojtk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3idnuzist.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3oogxqtez.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ecoawolh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hrtlstow.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yjgzyqup.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3hmvdvurc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lhqdxtvt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3iyhufdws.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmghwom.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3zmvpegib.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qdpipvlm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rifqkdtm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ziypbxuw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dixoaepy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ugkccauj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qefmufif.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vsnrketa.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3zbtvvefx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xjdigeqi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hwnatyhs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3emtqxkwk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3favyxnez.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3eczachst.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3fzcryfmi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cwduknyx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zrfspwrd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rwqzmoyw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3nvgvjkfu.html


<!-- 参考信息 -->