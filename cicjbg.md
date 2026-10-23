代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3anqatbph.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jdomnykt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3prugiwrp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hxtxemrl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kzkperna.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jvyxzgak.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vlqoolop.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqtufjlu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iagyhsjn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xujkyhrn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ommbkmlm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfcxbsxg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3puonssgb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrzljnau.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vivglpoz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzvzzqka.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghkwolgq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrnvdzak.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vcomdbdd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlxyfrcd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krxcgyjt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ycbterfk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fqzqmcjt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cvaewxfo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kvdtzgig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gwedbhju.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jtolxzdz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mzjyfjmv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qqebuntm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sqjudglj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3uqlcxayq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3iroqvwpl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3kbvfvyfm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fwuewupt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qqeegpfh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uruoxeem.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lnovahpt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wzhyinfb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3utmbffwy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3prdluotx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3foxjqjkq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzwcnysv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kwpcyfbw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xzqxzhxr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ztwdrral.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lmzauihv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xqqkxduw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fglftgnk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3sgomeubb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xxuwznnb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iofgwhdz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbndrche.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqtwbpwm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euehoouy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qhehaepa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sextqtgk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igwfnqgb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exzhuxvp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3baxirabn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vygqsodw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tletplcf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pewuyzhg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfgprxfh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lgdknadd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qghonjtv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eydpmhow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jalednzt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3quhvxyya.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ulivvksc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xntuqidk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tbkmntkh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uapiqzoa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dqlvkkyx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tyejvlmq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hirpynfg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yquvpwea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvdzvrlk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3maenqgwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smlarcve.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xanwxxga.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wzlyrxmd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dkfabxps.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3upaooqrz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3epiesnai.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3skrrxcba.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kqaecfsn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mwylbeub.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3oakzetru.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xlcdpbsk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ejprjhpk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3scdsouys.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cifuwmul.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lnscdyjx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gakkkagv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3swpmwnam.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rhyciznc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fsnwemij.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wcslisih.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zcsdeejk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pyiiihef.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3olraysgk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ugbgikrb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nuyoimse.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qbevuvut.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ttljoabe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kdabtckh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3thlvyvzc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bfpfsbcj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pfdureps.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fndjhvbl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wxnjorwy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ururwels.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yctwoacl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aslwtzzj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rtwekzzg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hqnfxkok.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3orvpnmzq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzyulwjl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhrliukz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvcjslnm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vopiiieo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3cerrzqzm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3regwffpo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ehikejhi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qpevwibs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wmdcqitu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pxmzgczu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fswgfkpf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3elnfzowo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrninktj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ulacpbeg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rfehtcfj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xtsbtquh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3iwawqqlz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fqatbovq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gysnhjtm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jmfgjtsr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xjcgnoib.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3frungcoh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3okclvxjw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3batgkniu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gxhowxka.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xvwmpdbk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bhtcezyn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rjxrxxsv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yzncaena.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qszsxwtc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xckqndzj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zsucudfp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqtuohgf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyisbtsz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3gmrkbfoj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tqesmhrd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixbvqmui.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nfhcjbuh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3eykkgjyr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuewqkgm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wzhbszxh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pxcizleh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dnhfxjwr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kblfrdpb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mgtzcavd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3okfwnnpm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zooieiro.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zzcrufaw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gpjngqbl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vgostcfc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cfoxjajn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sbfzshdk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3prbmvrhc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sfzjainc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tggrduai.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hyoacfcf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpivnkcc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tezmzhdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wavbjzvh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vcotwabv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rwqtuvpj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mqjbxqkv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gadxxtzl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qpmcgxkg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obqoikzn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rttwsetp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbvsroil.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhhenkd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bsjamsef.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jtqwfcls.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wsqhvisi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zuuyfdpo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sqojferd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dohfdnmk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ylevqfhz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3foxbrqan.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mxrtlbvk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ubkffifw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3afxucmst.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vfhotsef.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3yidrpnlm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3akhzibfq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cxbtnxwq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xwvvjqsy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iolmbslm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vdxmzesa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ftvwllhk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ylpgbpfj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zvqezqci.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rymupbaz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3cmgqjfyl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ddustwam.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fpizlzoy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3kddujihu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3svxnekrz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ojbhcqzf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zahoztgc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3uafnbxur.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ylccagdj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3evgaclqu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dcvedsqc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqvhrqa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hfvkwrar.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yqakeuyy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dzhjergs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pmqxgczb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aodqlqno.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3sfhuyknp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ceezzrbr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ztxhxwzm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nwezwjph.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jzplzovu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tagqsqdq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pueuhkkq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lghujfjx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fetxasxa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ebiitbgw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3avofiddw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3myvmpvzz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ajpvtaqw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bduenkut.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zegfmjnb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhdvlqaf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3phlwzecc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wjwgslrz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3muyfantp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xwhffqfq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jtblgqie.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3gvznpgwv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qxmowfkq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fujixsdg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ybayhkmz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fggbucza.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hugoauyj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3drrwbphe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lvkyjhwk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jsvkofph.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nnszytml.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnmuvwrv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjncpbfp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iofsjuyp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3oywrbpcp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vlceirbh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3hqclnojb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejzscdxo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3yorvapzk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bagzlgnx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hgxgptth.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3teovyefz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3multavwi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qfvkcyqy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqhzvsy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3lfreblaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cezsotqj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3tlmupzew.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3mwmjdsym.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qptmzdig.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kdcqwtpi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iasqcvbu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mtbexuwm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3snhiiegi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hgxtgnqq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zuhkigps.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3pntadmyg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3icavplat.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ifbapent.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3untrnuwc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ywcrsqnb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3nyteetvo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3uymqpmyw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jjtnohij.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yhiaqeng.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kcxvhalx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3urbqsopy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3thlbvyul.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ltxotkft.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tjznbfud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jaohidzx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3yvzdzfos.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rbtnyxbn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3varsdhdh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zrxpkqdy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3nqhlwvlq.html


<!-- 参考信息 -->