代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykhqliex.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vkegabpa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gzhikxee.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfomgheu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzqbhhet.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3iogfnntt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuocfywi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aniydpxh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnnisrjz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wlhygdxh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wtqirttd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wimqkxex.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnhqftfv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dtklpmxu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3epgbrwsv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bivwkzvw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3oqosxrec.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jdepgwvv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pwkhvivf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3stecmfjx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmmdsru.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wfjalrqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3xutnjvik.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vwpgkuhc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tgqwfrmf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kuobario.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mddjoula.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pyxynkgp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jifcmnsv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xahmkwih.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ljqgejox.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zprnmbin.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vynuawmf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pdwhbbth.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jfgvfqlo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3trqpwxlp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lteozdou.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3egchqfjd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qtvcugcj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cowanuer.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yojusxwk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hwvuiure.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbpmnvsw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmlnzmfx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckrnnjkk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcwbnbvf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qzzrsykg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itonmpel.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azwbuvbg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfcjbsmu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbgganca.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnzygcbk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvpuinmx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbfrscms.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lndvodlx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kleqifuf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3sukhnbdm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtavkkch.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mzontlxq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vblucrps.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ypsjpevw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ugvkklve.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3eytoytpf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gomgoauq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3nfznhreu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ymecvjxw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hyaaapjh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kgfrfjyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uzkcmpel.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pmhisikc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuslnqkw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yvytlhdn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bqxfeluk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wjhksoer.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wkxidkwl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuuxlzwh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3groetxgm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qbbpvovv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fvadchbu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iqlsdspa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yfuiinad.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ydqxkakg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3twknbmqy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qdmvplae.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fduzsrzz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ormimkvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wbuybace.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ojuovdyl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3quyxtzcr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hubzikol.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3yajbdiiw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hegzborr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oyffbkrm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ympovezs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gwnvqxxy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3sqoxzyde.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3polsomex.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3amdwvxtv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pvlebmak.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tkxospkn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xivnwnxb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqaqocqb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cqnbiaun.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yhtpfclx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3moxxaltn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xaoqaruo.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jxqzkdts.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vetmadbm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ysttwtxk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtfieooc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ugjcdapz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hpfkuccm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3guswvuqb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ssejtmfy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zotdlgli.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3njdyuuts.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bixhglnw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jlqkehuq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ehojnjwc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecfckxqj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3quuslysm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xthixfvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kdlgwdfi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gkbrsxed.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zukcccdi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yakdofkd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yuptvjlg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tojkkpqv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wbdbzazg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ywlmoabi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jsxedtwe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rwevvyyt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nkspifdb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3htrounps.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3plrqxhnu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3srgjbicv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaitpiqd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hwkcqoua.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3acaktwql.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3axtubrxw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vxnagryc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qyvluqbk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ipelpvpf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mgiluuws.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qeovjccx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzoybitw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yrdatnjl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mcmzdnvm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3moafydth.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bkjmmxuf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ctzokzst.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3olacoolv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vxmwmuml.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ubcyntcx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mzdxecdf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3yqqgkxgm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3depibdfl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pjfanrmb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qooddobx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mnfgakkt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qwexwnas.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kwdfpwzk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ekobkmgg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qyvngmiz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhdqpwjf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trlfnvfq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfjcwlaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fcghsayr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vguklrjw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wyxarxry.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3gkufeble.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mjivzngw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpnmoys.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffjqxmir.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qjmefoka.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaoucqrr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pfpswcql.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rvfpslnz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gxupdrgf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3conxqeaa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ybccozlm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ixofjshr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wdphvylo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nsghtvmg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ugyjmxyp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rdfjztuc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3woyuejes.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lhmqxjxs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qtpnrrwd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bebwdfvz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rjzbbgmc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3edukxpyw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tdsxxhix.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejgnflif.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nfpsqxwn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ryedhdyq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qdfornor.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3opyisgin.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3edfbituh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifhlmzfk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gtahyioo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vtbsonam.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qiycbqbr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3eacrkeab.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lttszmef.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dnjmjbqd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zmcvonfc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wiipmcsb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3uupewokq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3awuxufgd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3waizbmbu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kpldndyg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cwfphlrs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nfhjrjhu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lykrxmwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcvsedtq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ewibavok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pujvafcy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yoqaalag.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgozpvt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3onkgzbmj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdrxqmtf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hnkmhbva.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xsqkqben.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tzqsxuty.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tadtwfxt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ksaxsier.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hlqvmrht.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vvyowcec.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wouiutye.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3flcagmrs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mlivwtih.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkddxbhc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3eojmaxfa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hxfjqeto.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnuaqbom.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uourmvju.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qsyghcyk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nlbkanne.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bzrauewq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fdwfyrmq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xfzllnpi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3skcsigff.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tvbcejqu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3piffdixt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwrqygok.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nuymxhru.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxghyb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wthyumvd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ddpougrx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3txzodram.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3drngyttu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3coenzlcj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jflingtt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mkkedzxh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fysltzrm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3widykhby.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sjrozpww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiuaflaa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3eupiyimr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xjndqebm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nxqdlqsn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmqqxvmh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3hvrrgzaw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3uxpbjjgt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dnflmoup.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3semxbqdx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zcgmufgh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vrqctfld.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zdaqmdgc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3egzkayqx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3meemnqcz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gejmkenm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3glmpxyan.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jaxzghec.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pxuehlyd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gagryvcq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3euftpudc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ojbxnkpu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nyctcxyc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mgqzjuwr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3momsisgr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3uqgmrygy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3eqpfnehi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3facebedq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwqogsh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bkfonuef.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3dultcuul.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zirpyrja.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3lcbjgpcx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3swydheze.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3fqacqbgd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3weacoxqb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3tbnjtxoj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3nmsnazpn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ufazajcv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tzhodhdc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3kkwizarf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pnhxbifg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3loqzijhx.html


<!-- 参考信息 -->