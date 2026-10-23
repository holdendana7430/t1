代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtbfxcxc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jtqhgrea.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpupgztt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hpmeaegl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pktvipgu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyaqaoji.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3krcwpmgj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mscvcxer.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syunyacz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amfafoyv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3uvatjkqo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bsvhebyw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hnfqzoil.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fbnftkbk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mjqtmxvy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3luoxczmf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ddhyhjhb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3glizubtz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kdenazmb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ueooszrt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3keenljtn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ipilzdlj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qzauhekn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mvomhdms.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ykyrgbob.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ewlrnvkl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3asocvcil.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nzmrdljt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cwaqxitr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csxhzhjd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrcbwqcz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vwzzmitx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zceoddpa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dewzrytm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3htlfjmmd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wapuwhew.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ohjjhrbc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ngsjqcbe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfnvrevy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xfbccgxs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwptswgc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eocmaveh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oxfidzqh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwuvkqnz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqqvcbke.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eghncsmb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3aechyivj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfqqpges.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3urrolakg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pinktajy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azwwtrvc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxwdckk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wixhqzga.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3baakmsaz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ulacjzue.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3drothxyj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3omcntgch.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bsnpcuhe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3waebyebj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pqicrlui.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ojceonoh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zpsjoekr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bbvqwpgj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3huvemnoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eojaliaw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3toclghby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpapisqr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jquiluob.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3lucgbzca.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bfekkowc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouydnhij.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3djytpamy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mutyugjl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ecikgfph.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hhkvhfje.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nntluabl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kpvwogxw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ylxupsxg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ggangskh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fzriboby.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lelombwr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjaniktg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yffgllak.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ezkclfuz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ucgxdaib.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3soapqclt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mkzqnktn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vyruchxp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3izolqwsy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tmxxliek.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bgfdzstd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vvnpjfsg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wqnkswny.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zijuvdkr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vfenjbhh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qdogocuz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxctquvz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwyuxpog.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgoswadh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtqvzyjn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hbbixlyq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tfgqkpsg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qflyjmal.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3waoqrxwy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dripxnrv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3prpfiean.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppjyuoai.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qpnsgakg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3grckrqtp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wadjzgbu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zmecpjmo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wfenylfs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3whmuwtrz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vyyknixk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aspybbku.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eibyqwuy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yhobqpkr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icomjhmg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3opgyugrb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xnbpdslw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qpttaqta.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3yvcxqeuy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3oqdlhlsw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tprfptja.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vbjsfxhi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zqfgntwg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aoermgby.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qtwhutaf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3reukyzkk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3oeadwcut.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ghnpzies.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wsrgsgjm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipgmgcub.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3iiizwoxz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3oysbfjyl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mrabjocj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tcnhxeok.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zmmyjazh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ympbthth.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kkryzyri.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kbchjnqh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fahzdjbv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ywkrqhig.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3alntwqpl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkcxzuj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lhefwkha.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ethphzjt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otvdwfgi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rtonczmo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lctzvqvy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nbhxieil.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vhmsqick.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hhotrcst.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qhgijadm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3sefdnayn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zlhowudf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3acctbvvz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3chpfvpld.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jbwycwuu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocsvurkh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nafghezm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3slxaurak.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhjrrozb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yhtdlgoi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3axdxytym.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zxcytumh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zgudprqi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iftailrs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqybglbj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3peguozzn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uodjhxie.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3krazuqbp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3byyzxhdc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yrgivjcy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yufigozw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wkkxumbk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3silbvbra.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hxuxbjhz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hsvzjllt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3itiwkkgt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qvgwytxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jzafywxj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qaxoffku.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mxocqfba.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mnjixivo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sdcthhaq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ujgfjlkx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3egvalfxr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3yvgprmxn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xglyyjrh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tyjjermp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ipszmbtn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mcgstfub.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3siawkakh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mqpmepka.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpncohwz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aeypvtze.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3olcngfcg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mkxjmugo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkjaqtk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3cxnyrpeb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kiazkmjg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kprakyao.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3axbbhonc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ixbsomjg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bgigtwyx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hcfgfrfr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bzfucpeh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qcahekqa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rikubxfe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mgirgegf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khqlaiyu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gudvmjoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3giklgrvs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mmxszddj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yrshiayo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3auysfiqz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tnwogwfq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zwjuabyt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ihpvuagv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3abxmppio.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hwwdbkrf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zezcdftq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ngchsvnm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qbdbgpgi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ygyydhbg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqwadcif.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qhvnievj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pfgjdssq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3adnnriuu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hemsppme.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbfleblr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uoqavkjg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bqqejrxf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3obakbuik.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gjizkjcu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iwiuflqc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pyqqtleh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ztvinnlz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lmueewpu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zzimeurv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rdcalznw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uahaxrpj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzcomqgn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyyiohcb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttwoqzyi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tlvoavbw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3utgcwljs.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tijqurgg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsveqgrv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vibchvyi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xfshnenl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3slutrbbx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kjmsmizl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chskjech.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3exrkixxm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hdulklws.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3sfdmmuaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rrbidqxj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qnwffhih.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kmebabaa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lrzgmcup.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nruedxef.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oyiwcgsx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jvwqwlcz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3uubzgpsl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tmgfoyzx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wbdwjbaa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ktrcdjhq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3sbcyvovj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lkftxdmm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mbfpbwbo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ytxwsksn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rbvjoszd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xlsylfjz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cxswhwxd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3agbyrmgd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gbkwiggg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xuqjvhjv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zzhhpoxn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xrncrsrk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3odklybzu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3pyitqmzg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3uxascmzn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3geapzbni.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wnjuybjg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tksgijdh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xghqzibs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3iafrfsrl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3inddgetx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zzmfhhnt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdfzdlff.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ctrkapsm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3bohxhqzc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pulfrgao.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3walqvizp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ecazofhq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3gcfmlbfr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3amqinaww.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kvwrigzx.html


<!-- 参考信息 -->