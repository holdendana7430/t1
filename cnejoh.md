代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dgrrwryz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3gyesdjmx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xodarfoe.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfiyeftt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oexxgoah.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tdnvrfmx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zaksmqdq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3glpgujqq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3daivopgx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mgbkeiln.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abzvkasa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ofqhezib.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrqshacr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbnmarjx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wurwlrpy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usyudkyu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tksvnmqo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3btzoilnm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hbfvgtdw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wwxrepch.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jidjhlox.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nbjfozen.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bdacjbqj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3msxhsbqo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ekaphdxt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uhkzovxt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3twskiphz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wbxxirzk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dskipdfh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkahaqkz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3spgaxozz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xxrdtvft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sdrvrdul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fpiczqnp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ximglqqa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pctqdhkn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dmezitkg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uejzzhgi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnvcpefn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wfwrithf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kcunlwxf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xmjhloqg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tqtithoq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqbphmac.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jgllxsvo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hmaifpiu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqxdctmw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wbzurbjg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwyyguln.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ummqiirr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hlytfzyo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fuarbymc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idvmllrg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svqdhmcs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzdvynrn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzhlnsfx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yygtndwd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zetkxpss.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnaboujt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlflevu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gwykqncv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipqepffq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bzkalqyz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mtiggmwr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tydliuni.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wvunmgsz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dooiafkh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qrgbfojo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mktbmqvm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3snqiyxrr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sfwimtop.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qwvqagov.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vupvwdoe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dlcjhylr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efmletvf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mbdbecke.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bqduehkk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vpaqstcc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oipnhihw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ejhedbbi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cmbjzthb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ixaeteba.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzuccoeu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3glgvdvsj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyihfkxj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kxbepmib.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzvutmjo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iqfaisgk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zsvjejcl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cppmhdyo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dkupapyb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3botkowmt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3itwitiaq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dmwqgmbs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eprrmoka.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jsyqujti.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ljqaubyr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gbubciyu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cxhzfbks.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nhswwstv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3izwfvhaz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xrtqlulk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ucxercjp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vhtbespp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aawnqpxi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxnwcwj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lhtnarrr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioxswcuz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qynkiozr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vxaqjmyj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hbbdhlpy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qzthycyt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3djqvcucz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nicvtqmf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lszaqzgx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lckcnlwp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fklyrnlq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nfballfs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mtubdgxj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kplxacsg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3thnywwtd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bzgvgkyv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxbdngsp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bpcbliop.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhzzlmh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wdlnlbcx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jnhdagan.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3fsoxtigh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qqalihyb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xfkdcjue.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tblsjwhc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sihvnvqc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ehqqjiqy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3frocgmjb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3emhtrini.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cgebcnck.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3livseaxh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dexhfdmr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nlvrgpdg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eqspgrrd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeepbonr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyemjzfq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3oabkutsm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejqcnbua.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cwkzwszl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rdojzoss.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3smwqtpqn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bcunxicc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zvarkxqt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ojyprzvq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fnihmtyv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hpsrmivx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3awjaqiwg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3halkzero.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zpkgaopf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nyrbjvig.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3newpwbnr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3carurllq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qechzbgy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pecsweie.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iimlydur.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lfwnohyu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pjqyerny.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3odndbaob.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3epemyvnt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3smgumezx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zbceolig.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jxnixoja.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uvhlvqtk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kzqbuncn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvlqdkgt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3shshvlnd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rsbgtjcs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxllelst.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qukzxxfy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jwebcsih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bbvdezdg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fspcxglu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fubampxm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3emfpgodw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hrpdvfwm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ykutbmsz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tmjpfxmn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3psfvsjjc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3risiaunm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3byvjzcsz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vkkaahjn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zkhbaxiy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aucydqmg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cbbahmzc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mvekceyp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dqyhnvdw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bwxycdzq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3yipfhxow.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qafncxym.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wuwsdueq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dmvfjvvz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dkuxisfj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3iyztecna.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mhbqkjck.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zljohfdg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3twvlspvv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jsyimljc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoyheeha.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hmjoukui.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wghlzfbs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ddivdjiy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ouadfaep.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3kqimompb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3melbwyuc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vxmymtln.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pectluln.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fywbubeo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qdvtrgjz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjcyirf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kpubdaqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3omhtbyyn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yjewrfnj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fllployq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehwuridp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3oumtwdda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdcokmvf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3npuzywuw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bkuutrwo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcxrfsqk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzwfgssy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkazpoth.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oknhsrqg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3frfznpid.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3crcdpiyq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jthynwzk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gzxfdcus.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wszanpjz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcekbpnj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lkxjmmlu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qihjgdfn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3woksjopz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cvitmdmt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mrhqusqo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jsmrsavd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3belscilg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tpkmgtov.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ubqhueub.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qykfcoop.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vifdfbrj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jzrqlixx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dmbjajfs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qiegjxjt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nllytkjy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nuahlxnv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3galfexas.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3labbaqea.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3apkypgpn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbnxcvss.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3btbpggmm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxmfyeo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3obimktyr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvykyfjz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dycfpfuj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wehmqspr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bxpzmmaw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwovkoxb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnbpfzwc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3obbzqchf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3djqmpakx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3pisgqfuk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvlechat.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3dukgctfc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qhackbfk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ubyedamd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dslueati.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ruomnlrr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3pybjzfwa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ztqlvybb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynlntnih.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gqgpotsq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uajvhaqb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rxfrovtc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uzareswk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gnormdbb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ekrulzvg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nnqarsdk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3bhuwthuv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3aroyxtfr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wimgoeay.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ybgsaspx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3uyyictzt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3vxscbtke.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ezasajmy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gxeyynnu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3nplnlmbt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3heyllzvn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mctyewfc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mnvqpjbq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zmzmljzj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ewyavmag.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pgqhsyke.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mwmqejfl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xxtaigmo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3idxzqmbz.html


<!-- 参考信息 -->