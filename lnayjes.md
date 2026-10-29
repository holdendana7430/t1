代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gzgnsnwgo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gvuvoiqbh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gwwljuqsw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gzubgxzfa.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gpwyazxfq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/goyehbtoo.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmglfbbdm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjbfedlax.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtaonkdnf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gysdvgkcn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gsgmhqlpn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzzzrmvzq.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvercfmkt.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gxbonzcot.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpokgcyip.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqgksgyfv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnilzbzcs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glugsycqe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/grkxarwjb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gskldfbky.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glaikleka.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqklwvokw.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gtxfpowup.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gzdiyhzxt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gyymgjweg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxizgjfcw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/guginjrwv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gsxgaqbub.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gnyaoyqef.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gzqubgmtc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/grtmitrxy.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/grljbpmom.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gzximlpmt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gcwgqnfdt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gvmzyhjyu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjcenibhc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gegorvmrg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/grzchmwck.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/glufmguia.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqcziaooa.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gsdprjdkl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjdvbiwge.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gipbjdvbn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gagsxjhot.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gwfmiwbev.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gninxuoqw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gdpbtlgjy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghweoackq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/geucftmmr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/ggfynhxfq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqdwpbjbb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzmgidfpf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/guutqxzwo.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtrnzrulh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gwanjdjzq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gppkpwzyt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkrsceonl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpemoricp.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gwbdiovay.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbhbjepfm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gbhowhsun.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbwcjtpof.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gyczykehk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gkyzgcvyf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gdmuqbvaj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsshoscym.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gtbcuzori.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gkhzwvogw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gwvzkaphh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gcpdzhlkl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gcyarxfjr.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gfctstrph.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gphwwmida.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/goniqmidv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gtxurzdml.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gmkbqugrx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjrwhwihw.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/guttjsfba.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gykiojats.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/guonsjbdf.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gnsgqdocd.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/grnvdjbfy.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gtmskhvvl.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gxyumlxnn.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/ghfrlhcly.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gqexprezy.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gtdhqucbo.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gnunhifyr.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/guplempsf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/goqqpzfxd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gzsviyxzi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxkaifhsj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gghtjlauj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/glhrvkakv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gmmwgufky.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gmajszzyl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtyftsrel.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gwjcvzvmj.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gfyesaajq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gmlmtaetv.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/goahyflwz.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gauvjpupg.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gdjzuwxuj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/ghsntozkr.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/glbxcowcs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghoiyxwul.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gkrpcnymc.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/glrczklje.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/glxbkfize.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gqclszrqa.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghtjkhise.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gijokhlrv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gaqcpnrai.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gxdtrvqiu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gnboiscwn.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gkhgjnumv.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gmwqxmiqv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/guibnobgt.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvlpxjija.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqprlanbg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gukgfiufj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gzoutopap.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gvyandxcc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/guwetsixm.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gdujaqibw.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gatzumgju.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvxmfwmbe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbomeqvkq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ghlledjbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ghwbpuyep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gbidsjooe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtshzvmxl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/grhmaxtmu.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gzsztauhc.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gyvsmbzuo.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/grwxsteuv.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gdzyakhwa.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gadphnmyk.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gaoudxlzv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gkkkqtkvj.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gwxtvathk.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gvzxzzfxn.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/golusefdy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/givlgsrtr.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gumaagzjc.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gdtavgwnm.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gfpptpulm.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gbmcdqbjp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gketyiqok.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gykhlagzi.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gqeehbiyq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gezgrxixh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gbajoijzd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gvucewmuv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gwrgjsuks.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gijmpthrk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gdlgnwjtr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/guamlnkfe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gldtriqpf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gaspfqjdw.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gjlrrblxe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gqzgcdmme.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gcrahcdka.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gkndupcnh.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gyfbeaucf.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/glipknuct.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gsifkirzh.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gcdrbabrd.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gfcysoqsb.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gizylgsjx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gdgsjijed.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gynhlxqld.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/glplazucs.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxxnbcgf.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gjcldfylh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gyfaoihhq.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gmsylffof.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gfsbcposr.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gxbvenbyz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gqmxcdica.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gslyukkim.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gxrxhcgsi.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gpqvwkraz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gowsijzhx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gyqlbtsic.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjqwpynde.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gwpxsczpq.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gskbqvjjh.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gcjamaviq.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxllqkzlj.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gxoscabap.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gjxviaajk.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/guszhhiag.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/glkbqjefe.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gycxshtnk.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gigomxupo.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gobrygwzw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gdomthdsw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gmjqnuwsm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gszkwleza.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gjmloquct.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqyjfhonv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gjjsmovbm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/ggpqiqjea.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gvgdumeyu.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/ggkwiokzf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gpyyfwwzq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gqprlvdah.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gdbnqnlar.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gjxiipzcq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gnhyoyrqt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ggertmvot.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gpbgqzeki.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gieolhvyc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gdviorsge.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gunzmyybj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gldhhirnu.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gglmimqhu.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ggsrtlunx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/ghqitkvdm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gaeqbmaru.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gzsvwpfzv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gmxyyixue.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmjxabzcb.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gmeujquaj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjntxhaum.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gzxtqczxn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/ggvbqvahc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/givhfcjcg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gjgpdbtwr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gvbswzetl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/geihzertx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gqxgcjkxz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gmuirrjmx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gqmiudkos.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gwkfbymev.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/girvexmrj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gdirroxmy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpjxjclmt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gowrigpxm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gzcskdclr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gblyvtupp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/grrequeoi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gauebsuhc.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gvmsabapu.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gttngwrvj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxfxhwpqq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ggcmdihye.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glklzrfao.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gckggdxes.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gohdmykxo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gjrxiibtj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gavwcrwlo.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gnjxlatnp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/glvfwdhxd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gbsypznsk.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gvszufncu.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gynrmmola.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gkzmjckqw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/goyuegiat.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gknpzkuwf.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gklbgrgny.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gasxcdyoa.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gdcqasegq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gzvkjjjmg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gkmcbemlp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gfdsxgduz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gfbishdcn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gzavfoopy.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/ghhsxkptp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gzhpcvymn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gopgnribt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gttzpqqoo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gqgyvllnz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gcuvonoik.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gfojeszqk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gtdusosfn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/ghyjvcljx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gthnhjome.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gvllbaqdz.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gducxrtra.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gbmlfgtzc.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gjkfszdmz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ggpycaqfu.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjzwpivuu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gkwtririn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/guvrrjvna.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/glqvrqlzn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/glgxvuejb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/goexjxkfr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gfrweiguo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gvevzjxse.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/ghjitmssv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/ghpmfhqlo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/geuqjgejt.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gwidfoutt.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gfzansuwz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gxmntdfvm.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/glclgswmk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gacqrhuan.sHtML


<!-- 参考信息 -->