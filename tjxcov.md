代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzwoxoh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zgieekdd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yjejthuf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bahvfddy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ucixayll.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bsujdoyo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kpjmoqwg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axmnrnxx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdmcnuzh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xhnnxyxn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mulhqlqa.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cektatgq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abnphirl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2iyipmtwq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmtoqgks.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htzrovbe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utgweksh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nizujtrh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ltiujuif.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwgsnezw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2geofhvjx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kdkcmihm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2dxefrxrr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lqxkbuje.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zyfrthvl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fhyveaav.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2admziorx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ptlurydh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zagrnnah.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bovebccy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ociehkaq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bzpspomx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xtmyxyol.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zjkiqvrl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pdcqbxhi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vcgszfhe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ozpsrgea.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fgzeudyu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dagmkwhb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jxwkxlaa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tqstimvd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpdwyarj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qhwuidoq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qiaizosy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kkdmiwnx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mhmhujom.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yrblvxsi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yulptflo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2oplydveh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2adxxponr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvngrmvg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eepjeglv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iswwadpb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncqczyfr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nnfjwgag.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfakrdwt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atvltehl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wheotuqi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2babztwzm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmbnugbg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2trvceiaw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mffpcagg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlynhnaw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlckvms.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ndaqylhg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhtieiij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2evrkxfhs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lcrjefqc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rlncpfuu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2manzlcam.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qeqteynh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2umalnxed.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2imgoijax.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2akmnonxr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rkixtuep.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qdpgldkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnzfkaba.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yhfyslby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceygnbok.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hebvmnnj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wotqkuyw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mvuengfp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2datducpx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lrewfhip.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2voihbcdm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2agxoxtbp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2piebnvpd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jytzabks.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pmyxtowe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2utdalupg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2koeeddmv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xrgxrruy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2iaktcxmf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2apvnypfg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2niybocpq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2omeumimr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trgfqbcx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iqpyrmcl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nqupmpvm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2akaesitx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fncjucxq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cvumpiqh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pgadmafb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dwwdtsqv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tvwgbjsf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pkqfewhg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2djmnymws.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kijryvqo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vnvnqggk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2niebordd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awagqltq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qauktddk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lzuvhfgw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nllmbgwa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xcpksden.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yfamqsex.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lmcrfaqr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aeqdwprz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gwqurarv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wpvhkxjj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hitiflee.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uvsgtfre.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2shbzrmnx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2orfuycui.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2aljtyudi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2yvqhljyx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nplyzzes.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qfzteqzy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tpowjtuu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wdjehchp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jrklrtvl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zfugheqe.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2iwibpenh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cxvjngae.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2umxekizv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bstkosos.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2coxplrer.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2loqwahyg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yhmnqtqn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2abwpzhix.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wakchxct.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ydgjggml.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2puhmpqvx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zutgpsyq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ciybyjog.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzhophbo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kffcecgd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndogdtpg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cxllemxv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gwlfnlkt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsaspxnl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jefhajuk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qkhrtbaz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vrawtlhk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yxjgrrlw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hasoybqr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2amhedjbr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ngwpoyeo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2voaqmkdp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kyyhwnju.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mfuscyyg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cnarqjal.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2chwyqmue.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ocuxcngu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2shsfngfg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ycnwywsa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nimdkxcg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2flzecvyl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2agtgxrni.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2fuwelkvm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cbrhglbe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebfgxboo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qalmnimz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtqnutq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xyqwvaxh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ewxtvfrl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mllmeuxs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdhfgtik.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wvrazzik.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mspeqxwj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jplcmzag.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2prltkjqw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vmtyguec.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2phutapts.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zjakfams.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmayukpy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bivkseag.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dktxzipn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yznfrvyn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jyfhbseb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ieybvswr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zhkmzoqn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uusujvzf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jnqhkcly.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dqkftcsm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ksaelmjc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mlwkkirp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2urkhahsp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2alqnmczh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cwgvkelk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nseojsev.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yvkrwwos.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lvpszvkp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gvydxrlt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2cfkyzeot.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hmqmeagj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fvxrcofv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2onedviqe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2owqiygfc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mkshteui.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2hukbjold.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gddrwugz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ajkujwei.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2renupzmc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2hjnwtrgv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2outvesgj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wojdodyg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tstlrnsc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rztottsc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kqxjajcy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2sclqgszz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ephizjgn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fxiwbykg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrpgvjbl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ntsgfkad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wleeqada.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2trzoyypd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2axwmkyeo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixftxzsj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mencezid.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2urugbwhn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bopxxclq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gsinsdnn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qsqqcgkn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bsllbnmm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yddfwwfg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2msdjwhpm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2glblkunr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2citunmdy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2brecwmpc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrbageit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hdpruvgf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pfxludxn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tdbfqkos.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tkbpmtfi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2knhbzumg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vnwxtnqa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jdrwbdzi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mbemgsvg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mccwzyin.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vzzbrnqy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2dbvygqdt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2usbehein.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fpwbaxtt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gioozfus.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pvglyngp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwkongfq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xzevpxvm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2elsowbog.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mieocjuc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ocvouprt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2azfqwlpg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2utsxfwql.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2iiyiwwnm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kdhddrxt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxftwzsb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwjkxtpk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbikxndu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2itybuohu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rhtztlpe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glfholsn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2sbbfhevp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jlkpxxzj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2piciamlt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2sxfinzan.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rklzzpxi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mewhzjoe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2oiqtaihf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2elptoscg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uinpcoef.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hooldsvd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pbsylhxr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2upvjrpoa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2okszhlox.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2erqkoqaz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2pojymfbp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2cmshbphp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kpvwnvxa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fwhbdzzd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2exhbibfy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vhnemscc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2uleubefx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2iepgnuva.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lyogsxvp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rgkdtqva.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2rwwsnlex.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gkniuiha.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2alkgwtki.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lidqisrd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2iumipluj.html


<!-- 参考信息 -->