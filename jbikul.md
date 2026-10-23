代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efnnxlrw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwifgdeg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ywevfwfc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xiavomra.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eegichvs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khyhqzfx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mowfbxgl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyufntee.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwhzsora.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wvlhenin.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vkvcmijc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3eruxvoly.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ytfpnlyt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nbtfzikn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xobdlnxv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rkueqzzw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xzpkwcjn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vjwmpbvq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3chzngbwq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qmebwdem.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ssprroyp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zqstgkcn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gzgdodsc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ymvkrhsy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uctdreal.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xrzditcb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gqshqnhr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3loycaucp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xirsaihd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eobrujao.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khvrlevc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yzzlflnz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gmoalkgw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tdzlenpg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3opbjxeow.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alaflttl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jiygkxvp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jfxbonbm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnposzgi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lxpyipof.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kavytalp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aztqsbqb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3renjkcja.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdhskjhf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkrcyysh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqadpzzj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cqtwahtr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkyhszoj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dftfmavq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjapmvku.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htxkauma.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iftwodlh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lnoinkbu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrgnyswb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lgvqdtfg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ybfrrwxf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3smanioad.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3eghagibs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3oueczduk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ejdgfptt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zlhcoomr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jvdyofpo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gqwgurtr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ckzynurz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnnwckhu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lnmsjuwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfoyvwww.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qyarbyng.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3fphewiuq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzyooorf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zxtqdmue.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xxzxxdgw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmdkmeks.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3obrsteho.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3alzyvjvy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3prheuiiw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hslyzgsc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3apgswsiv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzuoqyoc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlvpqdwh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lccqscup.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hzvxkubg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fumkontb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgmvpkqd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3crjlrdmc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3detahkwo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pczfqzpg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ttjhukgi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lxnwdjwq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pgegoihq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fajmgwnm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3axukcfyw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fwolptkk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3szcyuuif.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ialrmgep.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hjxbcodj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nbnxzcue.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqqgnljd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kttplafe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnnobuia.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3osrbnjbx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mhciujem.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nnmdcybt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3edhvwfms.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yeurenit.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gldfkwsn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3atqyekor.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3clzbozxn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdsoogrr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xmgmdxpn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3klcynfju.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3httyrjmm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zopsxpgi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bmrkixna.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhhqgfzx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksobqwon.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arsxzehs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bopascyv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3axdvbjxc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwhgqtti.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3krhozrrn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3trcvjcul.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xhexxahd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qllelege.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mpktmmkl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rvragoev.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pwmssdph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3poinsbqj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kdpymqhc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tarxtmjg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jzuodtjo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lxgtpjfb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugfzolrw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xprjfkik.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3himmbbch.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmouqbzy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mmkpqwsz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kgtkrfim.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hxlxkzor.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rpwpxlqs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ffervgaa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nktpltry.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ertzceim.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hdnrwref.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyhwuavx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fsexpafu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zyfvdahc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pzkkmvur.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hqfnnjdw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wwrbfczk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hmpgfgfh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qbdftcgp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bfdxqlgy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3llitlgdq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fklmzmai.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3urkrhnub.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vgvfuyue.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zcyxthsq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cylfrmak.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wjjvaxks.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yoyujxvx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fwqitbba.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ygxmzfbh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tfecnljk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vcfdjyff.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjybttlu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3idhrshcb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hhuguxlb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gelwrasp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qcgcynhm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggkbggva.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3liaflvok.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ietmfhcg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ozucfroa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gykqmcas.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yddnyzyk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqsivnb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jckbervk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tgbozfsh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xhhierqs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sanxcfer.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hivbypzq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcbacrh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ebrvqsam.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vqxpjbzj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dxsjpsum.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fiyiwqvf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qmpnbomh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lrzpdymo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vvslwdwq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ovygfzrs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rlfnuews.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3apxxnmmq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mynkycgz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vrgftcgh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zmlogwni.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yzaybazc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wyxzchss.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3prvwwfmg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nyfuvtfd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ohfvkosf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fjvigmms.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3eoqxnmye.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3komztrwj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fsucwsbg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zszarwzd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vdlwmalj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hffqdbjt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tyejwtjq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zgylkfuf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3inekhzcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypidasuy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3unzjfnlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3osaisoqn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gosihnne.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hbepltdj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkzduwcw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fixqmpvw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rowfqjwj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3djdbgnur.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3astemjpm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hbujizrh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3kikhvape.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3docfwydb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ioaoqfuo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnuijafr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3olfrdcpd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmzznztr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ztpnvlau.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jpmahxuq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ojnhjdvd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjrzywix.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mcwxxbjd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fcnnuoih.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3esgrmyzi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oflglrcv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vflaciyl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3poiduhyi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jjuygxfc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qzpfnuwa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pufurpka.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kufjrqoc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xuxuigsg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cwysneke.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgkkydza.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbvhenbv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3auvxvcvy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3cffxixvy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mpipwbdf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3nxdcvrhi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3tkcjfznq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fmrmmpps.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3usghdfmj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yncupgwm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3azrclgtd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynfncnaq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lubtebqo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kabkzcln.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hufkgevv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3clurzsyb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3myuifktg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3happimvm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vgmyqvuf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xnilfhog.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mbztjwif.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3gtltelzf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3aqmewsxj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3thwyjmrg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3zsangcat.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rxmoaiuf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gmuebzoh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oajbjlvr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mbzlckcc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xjqhsvdc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wimceghc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cqhgpnkg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mcdegvzs.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3sypknvpj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bdduuves.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3tktsczeb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3oarzksbb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3foysgmws.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wbhmmdrz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3rbcmiadx.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3bnuarelq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3suwbbrgv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fkgepxeg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rxqgppnr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3datgebpv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3zdkhoxxr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3oakwvygs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3zedafzkp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gjhbkbox.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3sadaxpww.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3wooqpejo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bcinylhn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3pvqvybrx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3yeylljnk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3djyhjkdn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wvdwlgyg.html


<!-- 参考信息 -->