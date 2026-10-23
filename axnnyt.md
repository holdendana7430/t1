代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gspmttji.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xknfyvbi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xuguyeyl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mdtxqwom.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xioujnjf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fwppuozb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3chcsrhio.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hldygwot.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lbjfxgae.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vmszmolp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rsjhyppl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ogubwnep.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylpjhxdf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gqfwutjw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mwpjbjlx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hydtfuyi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntxghrry.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvzkspxp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kctvluia.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iphsvfga.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfismxhg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stnefvfp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksqokusu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjubrcyf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egbuvccz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nqqlgmfl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vcmwwwmq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jbxztizx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3rxgtjhoo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mwfpprqr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xuzfncce.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3trqggvnt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tmqdjala.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vnqpxbdz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3nrryfgez.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cmwrswjb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qyusiaqu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzdryorj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jllnnqyn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ammnkkts.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdgbbck.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dtweazel.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jtrzlzhr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ypotdcig.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tdftaabe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jktulfol.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kzljzeus.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3njxqvded.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cbogqmup.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sucwruso.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zspybiqi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxiulepc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3sbyndfht.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nhosxbab.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xafqdnsy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjxuiswo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycxygnlg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmrlivxs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qxekqycx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgkumzaw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgztzmhb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yydknwiv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymhbobiq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cyyrvxkh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rrphdsoz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctxoripw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyzicmhm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxvoogk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cloxjuiz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rrefdmml.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lfqczwgc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wfymbofn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vpswukuq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zlwpvbgc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3moxipnui.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gjqpozoq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fnqewcox.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3gdnaqcmv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kexlhleu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vxdcsyzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwcxzhqm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fkpcsnhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grdmqgux.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ntwirdve.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mtdqwugr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3iqhbnxrf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sftjgepr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywuxilhq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iarhgjad.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jqqrarrj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ieifubdf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3krjkzihv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mmdnmcbp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ahpfyjwo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nrkuwnxv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uusxfuzt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkvhxwrc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhwfutjr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ftrrpifm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xjfnrmzs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gyqpyard.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tzmyeqbz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ygzxsgsc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cjiscutf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3glpyfimz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zoozxdfs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jzqkzxmv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qvhrzjzp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ugthxrzt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vdnakuea.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ogmtzyan.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gadwfzyw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gecensae.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvykjid.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ptaawsem.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqkzjtmy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jxownypn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oetqauav.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nqrxtxqy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xeowuyvd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mwemjljx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zuxdhkfz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpwslvjl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvbshiet.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3psngenrn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qeobjlbm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ksrzvtch.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bwxqzwkj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bqzzliwu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nmlsneuo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnaehwld.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cscfzort.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucqullef.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csvjzhvn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bywbixmi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpoojvgg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oevcfbzr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3afymzgcy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aunnjeic.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ydaucori.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fgspulup.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rfpfmkrx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ihghegvp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ijczqeuf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kcciautq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3slklrbml.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mvatxvbp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3menljdjh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ifxtnudh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtvfiqyr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3komvwvbj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdqjbwwu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pdkkkdcf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fihphkbh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3whyhstlo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gqoxnmjx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ncrxyggs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ybcjhqdw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zkriqkvb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtjeurx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rvozpyue.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vwwuzvrr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eiatabxq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tfdsnfxs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3huxucbeu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ipwwlbcx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jpuuuwgn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hqswlxta.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iahxgblt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xxxvrnlh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xglpdpwy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uiwehokf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kbdkipqy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mkpqwdtm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lhllpgpc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuknecve.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tovuinzd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkomxldq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ixsbdkgw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3crriubif.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kttybbhh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ylbgorsg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bapltrfw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lckdlyds.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mcrkxmjg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlqwuoea.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3knldjrin.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dudsyonq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xkproxcr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ripzyykc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ffjncpfg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lozxnyre.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3adxjbwez.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zywrwmxp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fzdxrfmo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tifmaqsd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ucrjukis.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3iprcralq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3deheqnrr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ipqphewn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jndffnlm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tsrvatux.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3oemzbajh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nccavunq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gfuuuhzt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlufcflh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tjcfgxdt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zbnohimh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xujhweyu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3pmpfpxsr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3krsgomxb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpcrptwt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xguhtezm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ispqssnf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3iaquizbz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrhhcov.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3feysthmi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bfouskvj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bwdorwwj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3helyvcso.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3evaqmjph.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nflaervz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ugabhijo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vpeqsslu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qbyshloj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3slzethvo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3covbuwae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sndlrlvr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fclycmzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhlmuchw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3jkmlitas.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bkrpbkin.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ykkovmba.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqdrluxe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqcaijyc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nztdmtwj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lbvbpmaq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kouicgdf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3nljgjbpx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tbpegwgp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ctxegogk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdhvhid.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vlhhdoce.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyhmosrk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pgwdvtbw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xbahmhrk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3uljyfltc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kruzhfax.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uxzhcpab.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bvcigukx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mevrsrxj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vzqtjtlc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yiqxsyam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vatmdraj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jijtrpmt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uxkrxqko.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ulizjibd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ptoouwnz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xczxwbxc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3goeksxob.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajrrwjgm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wdigmigr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wulbamss.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3iyydllgh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3phlthbzx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dmivsziz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qzsvnbuz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qlyindcc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3geubzhvz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jwxxoskj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zuijtbvc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdkipcmj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qvlnzzza.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3uynjykzn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzdnoecz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bcvjmzsb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3dnzhpuze.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3unqbkqqe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xjsgtnrk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3akwxmyjq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qxgjultl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3slxhkfzd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3pzztknli.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yjawfjsx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nrrkjqkz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3trmcfigi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jbcpdewl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qbfiwwaw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zsqjyezv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3apjonmbe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uslgflfw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3bcaqlqlp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gpgoseho.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3yjecyyly.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wyllibqd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3iljsclfv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dfrchufv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fiopipux.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nrdjpqtg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3radtstqu.html


<!-- 参考信息 -->