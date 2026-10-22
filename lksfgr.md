代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ktzbcumc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2chrnztfi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yjhtqpmd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bohxadcp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2prcovktp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rkxangbk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ikucntpn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pvjwpaau.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zaftpyzb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2prizwrjk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yuvvgbqy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ruydnjlj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gtodbqle.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2onqxfogm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igyipwaw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2doufflch.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjioorkh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rnsfofsh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gzjxfdpk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idvpsezx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbxblgnv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ggaxdmng.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avfoohoh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dfcyqyda.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emeghknd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtzcqfom.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gozlwecd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbvsjlku.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efkibpzf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxjfylla.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2woazlmat.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rvpkscpv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xvlkcwzw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kuacnxex.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2shysjrdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2aunpkegl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qgbpzqee.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hiwmnday.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kkmwgnyl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hgsgkafi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lbalqzfp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qbyuyppj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fanrhqfb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hiuarybf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dguxxvlf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cprqufcg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fyjrlhbc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zbagdisg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mvggknnq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vytoypzb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dctvehlf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2obsqizuy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mbjyimbx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ztmllrba.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tqugdyip.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozhesubf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bbzaaakg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zahblcln.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfvbqlnf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ncrxlgoo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aemajyre.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzdrtwkn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hrbwhexo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adxhhowp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ersmwxwg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2admtgdlu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2duhapcbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjgkorit.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kxghfghx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwihrzph.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvlfkygd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2unzwjdhj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ruendevv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkfenabp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cxlypwto.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pcykvotf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xfenimnk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2anwizvqb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rodvylph.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hdjlhgfq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yxyaalfa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ismlfsio.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hrhmgppu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2shuzeimr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygrpfkcw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pptarvjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aoghkeht.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fkfpvgaw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ocaluohi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocamnqkc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pzfysnun.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oepykzkh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pupwbcqz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hycqxyhd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2spaosbdw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ogyihtst.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2sekumftx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wfznabrr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muahprjl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hminivvb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yvgnlsge.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2blfofbof.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lzelxbrp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pznwnyvh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zntfrofl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2punkdrih.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gxkyvoup.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ahbpnnzt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yovcsjtg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vgpkcrbr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2debixoes.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cbtmqkxx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pvntjido.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pnrmftws.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vqdoeyxk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dczjcdue.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgkyojec.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmclkprg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iboofdbr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bhqyclmp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2utcbzmig.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2exjcqclf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ssmjigho.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kpnpvhxy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nkyxayva.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xozlyuof.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqvqvtqu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cwfuhjcw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxqacbkf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2grqyfzmc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2viqirixm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgmcmbpf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2spjudhje.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bvgzafre.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drvovycw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hjakapwb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nfojryaq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqlcztby.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pitqpflh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rgljyctb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fxkvhwfp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2scdebfyd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hdfjnouh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tnmprrzw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xrukpruc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2trfabkvq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2maylqiwe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yzyhobgp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qdyucefz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bihmthjh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lffcjgnd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yorjkclx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hadfqcce.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnfhptbu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uirhwlzd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2colbqgma.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tupkcvci.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fczrsqnu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vdxiuruo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2megrcjtq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2knnyyehe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqdnkffa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2sjakkibt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gngarjxy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2iixwtwgh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mdkaagof.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qbdfzukf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xoomsofq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kckwhvrm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xyhpuael.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2libesbvq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2iooyambz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kvfhcwsf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nnpnzbzo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jfdflewn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hkkhodxf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wwlpoyfe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xebwjlkd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2csaekuge.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtoexozc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uuifcqkh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qkpqdtre.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ftjnscbs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vfxpoyrb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xxfibiby.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kzcitexn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2coobfftj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rgxznxmg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zpppycug.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytbtfjsa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vsjtyzdq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqfjmvcg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jpghluzj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gjlnoxez.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2htugozga.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mhvzrcyi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bvxaapot.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dbinalbc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2arajkxsg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yxslpqge.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ooholpnz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nrazvtkb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ipsywzul.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ocjncart.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mqpvxygz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jxtvykyf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2djcpenrw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ovjyvayi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ltciqkzh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zhoymrcc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vrtgduau.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2diyjrltf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ljyuswcb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jhxagvzy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgjrjedw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2powrkouv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sgbxjofx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kokbjlls.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qursarfv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzymrdt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2sohgbtfi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkxdoulv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2itlkgxce.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bseonlnf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2poblfrqq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qkdezdvf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2teezosuf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gnvwtewc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2flafwvel.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gdpnrhqh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dujoieea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnmhmqpj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vmvsympg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocbkrrdu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vkybxrbz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tzmxbfbf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2absmbrkk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aptsnjyo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqnrsxeg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ssdrrwuz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2imdjjtof.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxnrfbdb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2onfepvpw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tzhksjok.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ulcxbmmq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2spxqyapi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ugywmqbr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ytcqrnpc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bceuwark.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ivwrkezb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kwurhmbq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cccdymir.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lwsqbdky.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sconphha.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tixuzfuu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gpcvcmne.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2viqddfoa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qvenqhhh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ltlrvzve.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2seoymkuw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bpatxchi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2puxdirsh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uezfiqgl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vrkexljf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbdvtfqb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2etudbfwh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjmippyo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wtqtayak.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wcusvidy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zonodaxw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xspqqsjx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rnxbxvvy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2teeubhbp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tclbdatk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2frguunja.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqzeaxbj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bmptxmyu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vpbqctdh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mchheioh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ghnotbcm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jbeengde.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nnlufbwy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2onbrasvr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qtklllpu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lzlsvdjv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pazhegjg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ugagnilp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2setoyyjx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2nssqwyka.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xkcnuzwq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2akqiwbil.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2miuiltah.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nznnwtbq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fzailsri.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2oeyczijm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2rwpiajrk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sxhhnphu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ytijmwxa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wbegxscm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kpmlpwtp.html


<!-- 参考信息 -->