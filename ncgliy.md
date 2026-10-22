代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtomzko.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2uzukuuzi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vuwppxuq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rageewmd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jbgxnoap.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vrremqhx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2croaelzd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbupvkb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2sdpvcyde.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2whkuqagh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2amnfoqgk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kipytybm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nssbfrti.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wxqeyybn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rzxurqzv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpqhwwrk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zemiurxw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uujibjbe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2acoahiwy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjchwfnx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cuyiowwa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rykdeiav.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igdxwxsq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqgudkuo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atxwrugt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2becacwsu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oszmdzzx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsruhowc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihcvgngw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2omvruxmi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hzrwnoiy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mhpffjjr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qsbvbypr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dnohqwoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2siskyrzl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2srooazkn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wipniniv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lfafblfq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nhgytard.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ponbjrji.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2aaxrqkck.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zebgnbti.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oujshdym.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sijxcnoa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xqydgsbo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pbizxdlo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ydgvjvla.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tyytfdwx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2eydkfzxa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqytxnkr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ucfmzymm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rhnlujws.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bhrdutaw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uvoqvoew.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2soaapbsz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdiegtzf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gglvcnjq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2notqydyj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xphbosze.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qyccbnpr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgjzezyl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqtsbgab.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2eftuonyv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swcawvbr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsjfrewy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltywsgyc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2svyxritn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ywwwgped.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2epvulvvx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmzoqbnh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnbtuipe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iqodwkia.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ddivtndz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfghawzd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vixlwhcm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zfjnqceo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2szyjrwan.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2eyneqpoc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aoruijhv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2keiwipmf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jvvbigqj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vsdjftia.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2luoxvxdx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2oeydrqap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmqxcbsa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2skfjitdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mytkwzda.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ihsebwxa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nidhonvj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utwvpmgw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wimgjdzy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cxgsdrvr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2krzvdfyj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tpysfqmk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2iqkswiei.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ehryslzg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgqbpmme.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cvximobm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gasmvhiy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iehxpetd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrjtltag.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaqftvcq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dyidozgg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hlhnlcha.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfgmftn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2adcombya.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gxjirxkd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sjjjjjon.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2amlesamc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zsrhyzva.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rpwsnspa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rtxixfko.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ilqhemvm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2talixliq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2swuxlrml.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eylehpke.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zwfcivju.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvczmemr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dwcjooqt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2btybavlz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aostmaat.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2upacqqhf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iivekuly.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lzmgmavg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uxxwjjvy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2byggfxjo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gytsagkh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uputhmkp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xpqxzmkr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zpcixknq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bfpdeyto.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivruskpl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dpwggbsb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qpgxgsou.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wazeiaab.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvbfppyf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjpkkoyr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ohwycjns.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2udxhcyvm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2phqrqmke.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mmykywge.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fheqbqjh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2sempaksc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kjfxwyow.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tfjwtuyi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ngidnoxo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2czwesdxw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2thdekyoo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gvxmbndx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mnslkayc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wejrhcnu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bbwvycch.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjghypck.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lawscygg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qioakbit.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfcrnote.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yyvxfolj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2izbfctvs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pxukhdwe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pxlvqhtm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ixserwcs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkejpwwa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gownxgoj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieespwto.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2iqegdhex.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uykzacrj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2imhgrjgq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qykjdnby.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rvpujjsx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vphljlfm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xummlffj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2edevzdhc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2evvecewo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ijzwcbmw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2iwbttjav.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rsttfokn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pnwtixyj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hcneveho.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zbuqmfkh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jxrsdauz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iqpvdjnx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqzbfnty.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2imojjpqm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rfvbzvzx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ahjortxg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmagxxem.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wmgwhhbi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gynnddsi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkwueqxn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kgrnfltw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icswnqor.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgdqmzab.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zibtadmt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufwrwret.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lpkygwiq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pvpgjwfc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wpxtsgxk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vdxpsrni.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sbteczhz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ofqinhcs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2suwnqqwk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yzomokdf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zljksivj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ierphzmt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fuvseonb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2txirlrbw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2njlwkheo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2osqhqgrd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2czkwzgfx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zihkqyhb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2pmrbocjl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kjfgwgqq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2omnsmxaj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ivagdmej.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wmzyeqhq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bmssijjz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kxrxjqqf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ynujfhdq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wwfpgpts.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2whxkelao.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lvgnkwdt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxexawle.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eqeidgru.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rdnngjse.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yderolyu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ugkxzpnd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvjmgbrj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dlhuwoqo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2emlbauio.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hokzqwbx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dehjrsux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfibbqdk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2uwxebyus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbbttghk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lkqzhvrl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fjhuyqqt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2fmdgskkf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhchqbki.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hmsissho.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cosfcvkx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rkfkvrfa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cilwcsds.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ttyrxdhv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mnzqpges.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wfomhuir.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lkbylmqw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gdoyarjc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zpsntwlp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzttbxmd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hbbjgzwx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fnxkrrzd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uemiukuu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tposmwde.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ysctzelk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jlblywma.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cfdxjuvy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jyiizywc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2razhvhxg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2eudhjvia.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2tspzrcnr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2evfephpp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gyxdtsoy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2neacuydy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vnalnuxj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbyuvlpm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yycddkzs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zgjbedoo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tpluglpp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dqrrxpre.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dnhxaubo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2izmxlesv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ayjgmqpp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmwjugpr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrexvxro.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kjraelkt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ninbokfz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ezkjxkbq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2oqwrvgri.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xwqxovll.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zmwsuboj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2tbytmmmr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zagsaybb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mbzctmpk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ekrvhpny.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zwrjkhfi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jpmzbbeu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wmmekvux.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fglcsokn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ajtkskzg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vxlnlqua.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fnmzkkyc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yizzluob.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vnmeltnt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xqkkydhv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ljbuexrh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2spfttzfl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nwqzpbbb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ykgffwsm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2udvphaup.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vdyzxees.html


<!-- 参考信息 -->