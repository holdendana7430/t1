代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lwkeckzs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2khkscjmc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hoggilrb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2douuolbw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yxeiqtrb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ncfubwet.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2itgnrazx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnpecfng.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cbckdzqv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2poiagkjf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zmxhyluo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uhslbhem.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qhuopwws.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qrwgsbhd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rnmgdlrd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ncgqoali.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xxqrbshz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ghiazdxr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dtbqwnms.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldyysvwb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bubjdier.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lulfygmv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2oibdojes.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fevzzdlb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eeytnzep.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rrjgzocr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hytlclsx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zzapgibk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxofpzay.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcbiurxn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uxefeavz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whdmqveq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iahcqaak.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sbkunzhq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jlciiykl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ehyrvddb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ewxgrvan.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2enxexvvn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bkniymfu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dqfxotkp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vmxulqiv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hasfvpkl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2oopmmxwa.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2grhpznqa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mdqpbcuh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aexyvmmv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oshsivrh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xwbcxngk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hdsvvonl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jvgcogjz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cgitufmc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2flhacfav.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dcuxxszi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrspzuff.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2axeklkgy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2smdqupsg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uvlmntyo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lbnqguov.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hoclscks.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpdwgepi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lrfhbfin.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gkxhxfwv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apcgjrku.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wxmwfvtm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nobzfqxg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmffegel.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dinrxgvg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jazdxhue.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qiojcmgt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izwytfzc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vidgjlkk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlhkjwyt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2murwroxm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2shmcqfgb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2juyqdtvv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bvkqskzy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ppbuvmhm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqmoifkw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nyznwmmp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cmgasbtx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zvrfckbb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2omwgybjp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zrwnjtwe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ompsisez.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2begowcdy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lnbustph.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ibyowjyc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ekciyodv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dkwsmnik.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pkcigbjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opxvaoab.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qbnqdiyy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hvrhwusb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjzrknyp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fzavktax.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tmprvwjt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mbrujimx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2divttlbr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwjyligj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzdufptj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jjjnagbf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dztjpctw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vncbjkeh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jkmzonrd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kssgcriw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sslbfbam.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qnwnlxsl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2crmgbrev.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vruwugcd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dvoqvrio.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xvpydolk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zeoilppk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bcmswkin.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bowatozg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2oiegbbgp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2uwrtiudk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lmednqnn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ittbbnfp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lqkrkxqj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2maepnpvo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2briwiqtx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zwghorzq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gazegopw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jajszfxi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ewoowykd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gedvedhv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gltkjlrs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2izpciuyv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2igbgkxkt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2binvanab.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mnkjewlm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mflfskqk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkyqqaxx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2puuyajmv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2svxdhsxb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vcmgmukq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mzseenrn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lrkzxbyx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uilnhzie.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dpyffbwr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2velbsutp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxyxecht.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2leokntfv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2svkpduoq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2utmbixqj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nlwlxfhf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ifawbmsb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lwdbzauu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2prgbiodn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iqgbkpbp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iqulciiy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2atpkbhfi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mmeiotmc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qbklrtuc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bqcofjnt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nzuvbzjx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fimfaeog.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hdnkhont.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ejwgxjrv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fewpkvhk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2akybksnm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2akwpncvb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kylbtzuu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dkotuebb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pmhdjenv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooztvvpe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qwfkaicn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2kvfdxdac.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rrldacgr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uhixosls.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rbqyyqqf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tbuhgavx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vxbqjqqm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ealruyet.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uikufpba.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fvphfecn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jzsqpdrf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ewndrgrq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bpkrrkhi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hgkxufuj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ubxcdvjw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nwrdxegs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2yzvsqdle.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zwoccpsu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jscezosv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugjjtctl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pnsmizrv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ymymsqeq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ngjiweji.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkfldgvu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rudqatxa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2skhggaps.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rscmaokg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vyvorwok.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tneqduqs.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftaxdvnj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tojdojky.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkqxzjxi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ypwfzhhj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pxbcjmjl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfdpczw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zanklypb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ogpfbhbn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rlufzbpd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qurwvkem.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2eesvvabh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzilnty.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tarvqiwy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ihbpzroi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fojtnily.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rfbkmrzc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hmteurtj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2veqdjhja.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yrxelrfv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2hwbqjwra.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ixrovxfr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ffioomzy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xykfiulv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uwgwrmnw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyycslkz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fkzkncei.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ijmbakqn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gbpmohfe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lmnbyusw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2upsokson.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fdpvyxex.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gcxzmror.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ycqbjsnh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gbovgiyn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjouivxw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwbqbzvh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2heamhqww.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ygjhxzsi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rwzewbra.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2pszucfbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afqkfobu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mfqrcqxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksivkeps.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2frxdetjf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2afnpzuen.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yevjudhb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpfxsctp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2omucbrbw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohzaalfo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2sgotarkp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pnacrzap.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jljaitzl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yzrjyygy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2yioidmab.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgebypsw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cwjvysic.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzxjyjqr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dkpbualf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2jhlsbxca.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ulmyjptz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkbupnvs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tvwjknkf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ubomdwbo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2naosgswd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2majxhyzz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dwbmyhjv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wbcizmcf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zlocfzan.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rvlgeayb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2npcidnyo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jwhashsp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vphakyrx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwasmbvb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2skdhtxip.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2owkntnjv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmplufsz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nhauctwy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jgwguigi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpqtjczr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xtepbltd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2htcwoucw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2gnmrpfxa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2chlwpvls.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxwkmgei.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvwlohko.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2aixkahbc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qvcmszgw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2agiwimsp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2yisarvtt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dbiabzbx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fmynjnqd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mzdhnmis.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2thjzmunh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2eyqviuul.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2nsaeejzq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ubqukfbc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pogymxuo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2esqinsdr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vtvjrrxn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jcnqqqcv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jgqsyypj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ketajdnq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rnefgwhf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ygscuukh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bozvnzuk.html


<!-- 参考信息 -->