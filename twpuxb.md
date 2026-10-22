代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vpdacwgx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dzgdiysy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cvfgwkuy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2igezxxzx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pfronmrl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2otfldvrq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2owcgemtx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pnlxpkwx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gymgxrgf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2drdmgnga.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2quvsgyly.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2giwvndqz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2faovbbyf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rqldcowp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ammixqim.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nikqmclj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzhygtsp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nhullhoy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfvojiie.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lvyfsnjf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfbpvswq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ednwajls.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tvmgudhw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnyaaygq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adljopqi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2stpdckdd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qzsiisci.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lazlcvks.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wcbkizlr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wzhgkfmf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bibrcfzy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fbkthyyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rgfthyjg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2prmswysl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mfdqzomq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ttnncfns.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rwvoxkdj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ltvxoatt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2robockec.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bchvbymn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kvsxkyks.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2woajcgdn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zjuftqps.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pazwvmph.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2latikrcb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zymskzjf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcwefjpd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nukbhpsp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zpdhmmwp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mpgvxbeh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gokqnvem.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntxzhdoe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sqrbrmfl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qsevxlsi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejascmdg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2coavxdfk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuprrxnz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywtlibxv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ufchsuet.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2siqhxnrp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2psmihrro.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkdjhjek.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jglagxvc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjqlysme.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kmttnpxl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yezhavle.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vcimwxfj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fymhzymv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2aixhrktt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdebvhxg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2iovyjfpp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cxolhxgn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zyhuhuzv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2iwytxqpr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ewgygpqp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2smbzzckd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2doptcphs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qfarczyz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qcvhzqcl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2edrkagng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmfuaruo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xjvebbsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xixtatym.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jxxsella.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qxatkwtb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydhccwan.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cruofozn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ssdgyzuh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2grisbykd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vxdiobyr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcrozlfv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yoyefstv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2icffqhfu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ifkcvrpw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2chwywhwd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ogllyqrl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gxmcpocc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcjjqtse.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mnjbbdwo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2clodywye.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2boxrcjmd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2klcotujq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xvvcanun.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2efrhogit.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2snptxdrn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2etkaeodh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2goxvwfeg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2luvwlmml.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lkuyhtuu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2huqnmkix.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lhmaxorv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hqmnqxdq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uxwkcupu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phhtlrcu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nsezabps.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xlxdbgsf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cxasrzeb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2agceozjx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tfddhpqa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yjccxrqu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2srxdwsrq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrhuqggg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eiaddzhv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wixiafvy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ojhdcyla.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2owigancy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ermozjdp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpjarozb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2apgwpfae.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jpamuicz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ogvqiycc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lgbzilxw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2okekjblw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugnjglly.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ldqtqdoo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2novefzjq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2itlelxix.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jkuktbcz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rxssirfe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xwywsnir.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ziklqjhk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pujhzgpp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ejpgqzal.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nrsoycps.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2nthzxnun.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wzarjqxq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wyzwzurp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mtzsvjkg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2swupacnr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kosuufjn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vjuafwtn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ptkpmnij.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2otnhlggn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2aymerfxv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qcyntgxt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gyktusgx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mxrcppji.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yelqywwg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2apyrjvmv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2imgunyqi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yitdvdij.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2miducrxz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lupmgnsr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnxgdhlt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hmgbfhqb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sgdrbsbk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2opvjhhpe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pidvofop.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2voaxbmks.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xnjqnavt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2emzojqis.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pguekoyf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vibtgqqv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2crubkrbs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hzwubzoc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fkutdbta.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcefmety.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gftqbckk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agvujkzn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2felmywel.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2alzzhjgh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmwpywfu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kcmnhhiv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2baufnxld.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqjirimp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eknvfnne.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pmarpeld.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkkkhizl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cvishbeo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jaulymak.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2suprhbca.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hieydiqt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yiufbdvo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zcxyhsrz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yusgbfsz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sufolxip.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yqpbqevz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kkqpjjnw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2uhmnlfyf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2boqdqhrt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2irtycbxf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yhmjculv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lmdqcdwr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2khmkvbnm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ykfxlsui.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xfakzdtz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wwjhlutr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2suocojrm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fwsouepv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wsuifwcc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmlazkvr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amurxslj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2iiewozjx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eqyiqkee.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nrsyixqn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lpfetvro.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mjrokmmb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ztdwmbuu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zhvargft.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2akefejwi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2yuktlovs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ouiusrsq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2orwtbhyj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yodyesln.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mghqmehf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2urvkoytx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vjrjdfjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cykmgcdr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dxjnyfhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qppczsyu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kpmqyykg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2aaqtjovp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bffpbjzn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fragwgyv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcidbdvi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2txyxgagj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hkqlulze.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwwhdxgc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2oqjbtxeg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tmoncwza.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tjjftlqo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cryaupqf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bumeelwz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fcwotybi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ccgqkodb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pfixnjdu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmemjxvu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jifexfra.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2liaoqurr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2hjvpivku.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2artboert.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2flucmuma.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bodjwqtz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vdtsfrht.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pmysmfgs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2aogafrgw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lptembrv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2atwyrwgb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cjegmpwj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tsanuraq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwstkcuu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wsqfahmu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwppxknt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nxmtczoq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2iamskmta.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lrnuyohi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gtnfqsik.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2esruzgif.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rzcallhz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2noxcqxiz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tdexbmuz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vcyurzed.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kggbpftn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2klftydfw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rytzxhwp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2huhgfzit.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ptkzyfnj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dqvdfpos.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wrulkely.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qptuydha.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ykrqpfsw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ydotaqpz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hmgrkdrl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qejdxksl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ubhgxreg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ccwdjgxa.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gbkspzim.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ssvebnra.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ttxklzso.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2knnymnfz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gmotsdds.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wyzbznoq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ohtbazqf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wktcdsem.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zcosyzuo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2afmafeyu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2xovjddty.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kbazlkno.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hgupvzpp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2pztucesa.html


<!-- 参考信息 -->