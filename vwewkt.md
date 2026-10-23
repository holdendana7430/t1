代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vrrzzpav.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yrdvufai.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ripqjeew.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3akcdxjrx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fejnaenv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xtbdkwky.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bzfoovyt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqwynfcx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voquvcgc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ifcxwaia.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lflikjzh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dasasgii.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhatiigg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jbglzxuz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hyjnlaap.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ymwiqizy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aixpoigf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dyanqiii.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yphyqyit.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwfkngh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiqfcsbo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evlddndz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3oatfbsgb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3thdfwrtq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fjolcnnb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qajalzir.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hhyqmwzc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lnixtmjj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jubvqwtz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3myysfqzc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pcqnptya.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jzigqlzo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ewpxahmb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxgejnly.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hdugcdhe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bhchwzio.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ywhotury.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cbedkngj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mmpefzoy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wfblferq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qzykclul.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3baecvwbw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3grhkzahi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xfnppbvq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zpydeofd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gkfwtqpu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kqvtdrzj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmnpshbr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3egqusxxy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nsowuoqe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpzhevld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajkbczwa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzugovmw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdgvahmg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3oidpytdn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkvbznjn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snxmynkj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcdanjxm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgnzvepu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acqcqjtl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xerewqqk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqxpzuko.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhpqrfkj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hcxtdbxb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rdhzwdgs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wktnwfwa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3iqztskpz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dpelvvtw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3evmbcagq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bmqkmdab.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vjktdqep.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3updqvaop.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qhrbyfvv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nsjvwdog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uemaxzmf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bfsahgou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uavbdbwp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tbrfoosm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfwjykki.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bgkvyhdd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3kgcaplru.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wyqekwfj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aclcpaep.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kixvesxg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xbxbessz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xlavrecb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3txahqbaj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxbuttxc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pruppqvc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hasgjgzd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byxrxrab.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmngpwtj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrkhcchf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pdvgijed.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cwtrrbpi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lkbmlsmk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awkbhwcj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wekkgauh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3luozhszh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3emvggwfi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tdfpikfh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jnbgtokf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3louyxgox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ktkpyqhz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dxfbogzo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zfwoztmw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tdpfcunt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wppxkdys.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3umhrxhjk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bffafhzz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixhroimd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqrmpesk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jixuffha.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrknjxse.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oacgobjs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tvdaazit.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xwgofyxw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fkdqsabs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkurruag.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3djfxxlqr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3roxbtlfr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wplodibg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ecwwxnvi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3owpipcyt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rgnwqqql.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tsadbpxn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mrbdfpav.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgifpncg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ldczbkcy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xctahxqp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ybyvicko.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mvvslmbq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ijyxjqvg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dglakqbp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3esjpgiix.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jqgrsoje.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ahxkndzs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yarofgii.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ypvlodqh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ejecyynr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mmvyepfe.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jdaxsmfn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3puisfsdx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3otqnolpj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3owblyerl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wokgvaag.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gyqqaark.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3avsqogjt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3osyusmaf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hnwfpqjp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cysafdpi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zsvxqtjk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cqtoxlyk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcadymya.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jxuulvar.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rkndngbw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ydykvggn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lpkczcvd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pyszectv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqfjqpgd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3evewygjp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xrqqurrr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ccytfkrk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3cimwrygb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3meurgsmd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gkcpvalh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lurynhxq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ymziobda.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3izccrcpy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qoogdiip.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3aalvunyi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfseeuqs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjbqmush.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ozcgwptd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aantisyr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kgidakuk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cjfyqfqx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3lreqbmdo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hphchenp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3njaepomj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rpuusxvj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsyvduxj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpjzjijc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3afufzmhp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ezipekco.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3njzguemm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aaoqynfx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxhemtxg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ajvflnmb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fmxcvivv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hvnxziyd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cgguhcnu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kdgzmvti.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3utdjapts.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tzkihcof.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hinvcqss.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wsaxdukz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gzwfcvlu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3boczwkgd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3truoyoek.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ishmlapn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szcbgxfk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uwgdfyor.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rpkxpums.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uytdphha.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ytakzbgl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xxghclub.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kakhcmug.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ubtjcffm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wiomvtei.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bpcvqcyj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfmgnug.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nvqafdks.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3esyctvlu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cyvlowzz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vakxzlpl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3unlmynkm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qgtowhfg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yzinwtsi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pxzhdhny.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vifalqcc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3inriudun.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eegkdvkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3murxvbjo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xwahjonw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rleoueao.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lspyrwjw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mqkhricw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpcjlujq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3egraupek.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhqcxxlt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kjzclhrz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nubvcgjv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cuvpyjkl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3unnwgnaa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rdrfnqzs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3limzmpbg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhuyeemp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fovojxjo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzcalju.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtyelruv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rbcjuqyh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3tctcsutk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pelktdfo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xngljtce.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hwpsxoco.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rahuiazl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xkukinay.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nrazbxmr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3weschmgm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fxwssvkn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xdjgrsdc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gkkflqji.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3qvulvvho.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vvrvroct.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssgzxmlx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xrnllbvr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfekyjbo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ysbwpxmj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wsewwqjp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3yaumvaqo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qirpjzpd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jmgpierj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3yopnmnhl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ihfwywcd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkhwvjez.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mhzjbkar.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nulsllcs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zaszzndy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3iuvfvmqg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3udsigmbb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jkgmzkvn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lnpmkusi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3apudhjkq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3czntzypa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3legiflui.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3phwhzemr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rqkibidr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3hrfktzmy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jucsrfvy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ryprsrnx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fmbzqaum.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3anqwnrcc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3emqetwcr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gxxtcjvn.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3cphubrtp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qwhsxdwu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kevthpce.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vvlxbxdw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fxcfdqwo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3pzowaeyy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lvqiurlx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3glngjqwt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ljqfxgkg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xrrugzdg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lunwwcti.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mmhcjdqh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3kkmqconi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gbqdnjtu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kazxwuwg.html


<!-- 参考信息 -->