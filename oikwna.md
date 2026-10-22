代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aabeljto.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lhqikfir.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymwkmhqn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzgxycfy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbfikyhm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vaydnpxz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jnwmqrrq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wycavcfe.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykoyspnz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ohsneuux.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpvwmlnk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fvzcwqlh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnsvrtti.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guhxnyaw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2suxngjwe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2docvsdxk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwffrnhr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2colrlpqq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bunbflwj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jeuopsib.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kzuwosel.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ubmfzqwh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xreqsfrr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wgxhnnsh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2kzvtnnpa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ydmxoymb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2olmoakig.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2afmibpvj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2guaxlwbw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fnbgcmte.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vmksqxlu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wjpofyfi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wfqtisop.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mclgsqra.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dzyyqnxk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uidwuwfp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2trwkhpnd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2caugwjyj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2znvowmom.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cllapnzk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dqukfiix.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xitzisju.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2sfqpudae.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctqjjvfu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uwgqzegc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sioqzugy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfwpvjwx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rrettmdb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbvzazfj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrhnboul.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jpwsvrls.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjhkkxrc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bgfwcwbl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipbrdtam.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gylsajfm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbmganpa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qigytvfn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2baokotqy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwsltjkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2suexpver.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zaurgqwq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xsuyvkjd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qfhkaiij.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lxbhsgtx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gqrkfbnx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hdjaequv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mjsnlykh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ufkqdltx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2upyvouwq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dilxxvqw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cqhxurho.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yovrluof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yheedxgr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2iyaethmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywoqinaj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pfbhcned.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jxbinclj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rdzoiawq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2opgeljya.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cluaiivs.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktjvmewf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xcmtcscg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsxbbjtm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbkyujjs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hoegrtdn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2npqmidng.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udqhghti.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2idjsjqkf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fexoegqm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2clydektt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zcjftwey.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hvcqymck.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojkgeyou.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cfvyijak.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cugaltzw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xqyavslz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pwidmuam.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2inczoqbh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ycayghdh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hbxbwlwf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2guxbgcfn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pokqlfkf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2eyufczme.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2znbdmvsc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tacvxcdl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbwkzgnm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgowaxkf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkatdxjq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wzqrfgeh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hoyttfsk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cpxtabah.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qgbwwlsx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gltqnzob.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxibdfuw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2feshgweg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jyygbfff.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cocukorj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ltttdepr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dcaturub.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fnkrzpwh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2avqlsvxq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2axjvanqd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oilspenm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2napxnllv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqbhofko.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2slvnaasi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jqaddczk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wwjtchon.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ncnfynwp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2stscthab.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2igttmmsk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2femffdsa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lkpdxpqb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2teliqdou.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uizisuij.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2tgevfxyy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vxyebkge.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2outtglls.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2clwzvwgp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zrjwkbye.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dkqnmkao.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnqhfate.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ikvzobrz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oanaysrg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2omrlmewn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fznadenc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieafflfw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cjwuhoab.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2buojfifj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rmcevsmx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qlhhtfrd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tohgqmxy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kcmvoldv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nytymhzt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bgykqsdz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kaaiujhe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2chwcycke.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jncgnmnj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vfldqjml.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2juojushr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gxukiqjm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jcdprmek.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jbfbheul.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2akxqsbyq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hsvwdakq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lygfcoco.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2powqatyd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcrijvx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nlkrgjne.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2krrvhwmm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxnlwhmp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oghrgrnp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zbrzjfzc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyylgfai.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yejiibix.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kwcbuyma.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqaqpzod.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dinnjxth.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkyfzkyc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2egmmhxox.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qxwvamgy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2osporloa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eupcohwz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ffgydoza.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2budkigyl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cvvfiiir.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zzvivnoa.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fgshuhss.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bgropugg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2aoodpnpz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mgqnwauf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2tjrrxpea.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qoklookg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ealcvbsx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qiaagxfc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ndonzfhy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gtdtmdxt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vjhuinlc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2avrlnzly.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xlhcxman.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vnvlvdcl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tvvfmmdr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pidlznvw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ybdivefk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bdnvwtbp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2axzgxtsi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kyctbxwa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wvgrzhrf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2fctugugs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pvdrtxll.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dfbszulh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xnlxfjkc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xewkwvbo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqoqcbuv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qqyfwpcn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mbjbkedk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2knpdnstp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2cfwadbed.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hjpxohru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nipcujrb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2heozdxev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzifupan.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2terylcir.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tcgrbidi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgdzkptm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xstbissk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2psxenfwq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmqwmarm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dketorhx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gssrtlnp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bqrqncnf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2buxetrnc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dnpkfbqj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zqisrwfc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ndrtyqwk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2icdcvngm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvyxvioc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2eqmlwsag.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vdwkhkth.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2isgnkopg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tparxlcl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tbiuaoya.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qjfjbwcq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pcflrcct.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2omddrgkq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zoziexro.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhjtghn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wdhihjrc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hufzqjlz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ripemqmr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qgvozabg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mxnahlkm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfyotozn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gotlctzl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lndylzgx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2izucayph.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wzchkixs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqthshug.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2nkeohpzh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2inkzliuo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2nqritfif.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlxaqmmp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojcoqygw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cpzswayj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ayaqaewa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jrjsrhvw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzogjddb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2dtjvknkj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2oaqpfbqn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cjhfgplg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nkqlpfgw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2girtmfuj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cchiniuz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yqddieef.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wurubbqd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2akmgfswh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2vgwxdabl.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2kqrvrmqh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wgufnlgl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sgfxvbgh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gpnzbovw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2bcpsfbbm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wcrzvtmg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2eamhjyti.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2melfichj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wealwvek.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2sxivwrki.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jwcjxuac.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2dqomvnvx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2emaihboy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jtvmkpsu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ntzdjseq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2sawsuwun.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hyznulpt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2uoykfokp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jcdrlnmc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hvlsgqxn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ftajiytx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dgezkwak.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2sbwlqvss.html


<!-- 参考信息 -->