代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tvskgjuq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jawjbnev.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lppoxpkp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zdvoitnp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iuhatcbq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rdxrfseg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nvgipkyy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rgfhurcx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qknwwizs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2czjdrnux.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fbidqgdf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ersydnzp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qscnjltq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qyuqhkev.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bicjdnfx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kebowabo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wzqlhwcw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2larfagcm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ctrttbzx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qzkxxvei.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2udntglqf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ftyukmkb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uoyengxo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlhghwpu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lksfgivi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rbkopxrw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vqyirrkn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2insxycjl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2coyikena.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2brconxak.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcprgoqi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fjnsgzoh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvdhwtdd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhufrcrc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ecvmpmhc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqgggvpv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwqzeoko.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vccmnxqs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2dejjpyps.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nglmtjzm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2krdnrjdd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cpmjnxyr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yplereud.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdsrohbg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrnlawm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dzsgazlr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2oczakipr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gdkdxrjk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2riezdaep.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dcimdihy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2usyhjcxx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sdohlnjd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vslyjkkf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2yqolxvph.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2jdiixlqo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2isesvmuo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ashtlzwl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdzxxrmk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qtvskbeg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vlwttoxa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zjvidrzp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tpqpvhak.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rippzudp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxxockys.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qfnzqsuh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xkjqsrgm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afjehmsl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ndnzjcmt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgrgehhg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cudqiecc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2epjanvdz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjuctwnb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itahffeb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxbtccai.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgqetakq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvhvlnpu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfdsuiyq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcsizmik.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qikhrsvj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rcqczfxg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tijvxmig.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znkgxmbd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hoymdzvq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xikndtej.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mxxhgedh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cbhvfrsg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zjyiqihq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dvivjbom.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2aufjcgdc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nyjcarzu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vvsrtxpu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gzycnsmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2buqmvvha.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dvcpgajt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fscwdfvs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ffrhllpv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mwsavpsu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwzmlyyq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmlasroc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2strllaau.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2txvgiwxj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2abwpkbpi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sgnvpsqp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2azuyxxtd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jscdckhs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2msrgfriy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obozcwzy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wikqquxu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kgtlplrz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fwkilsqo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nqbppvtd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mbbardpz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2omsdhxdc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ozniplkc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wrspakls.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2binwzexi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2thvvyhhw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2snswetnx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qatefvdf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bhzufbmk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mlcoyfmx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2imcqjcwk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cyydmllg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fnoszzym.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qmekcgwg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsxsznf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aiziztpn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vjgrifst.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uounmlyq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2apaydoba.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ksvuyuvj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2clodqhsl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2udlbocco.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kvawqrly.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mupolsja.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vparfvsb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wybjwuwc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hgptkpyt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eezzgejt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lflzqklq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dlfjhqcl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kmvcsyfp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qzdlbrqg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fjefjuxv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2refahhbj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2megpvwok.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vsnmsypw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkgmlhes.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2aorufpcw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oncbuofy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rfrkzzji.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qoojqwgg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lhmffpkq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gveymqjn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2npojvvtm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ayrhdqij.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2asvdctyl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fxfqodvg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2iqibodpv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jniolsbu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dhoamaog.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qghomqez.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohxmiirk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2adbxlonu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tvomcwdb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tsijufpj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bwiejecu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kjzrbeyj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rlswvbvi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2znutpjeg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lglxyegz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlhcxhie.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxnzmmqa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xwkfjgah.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wblfsulc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqgkjan.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rfnivvbm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pgukngnq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2upefgdiq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dfggsrzw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aokxmezh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gaywonaf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fibktkuu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tnfrxhep.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uvnkrvup.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qyqpiavm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zdmwxgcf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oixxlkii.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bglcxwnl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dhfynaln.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anjmbgqv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cykgywrr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2aloutdtm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2obvyjluc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mtqlozuj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jgfstqsc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2defsontq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgvnighc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwhpovxy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2shetqbwl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bscstkca.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpkpqqbp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jaucrklo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lsowyhcy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tlrawbvk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iwzbxspb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ormjtkfu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tacfrcnr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2azvjuhdb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bttdzsvs.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pnwvfzij.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bgntqnyl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cnaytljn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pwcgpxei.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xkbjlxfa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lhfrmuro.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2voqpozte.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uacfizur.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbcofql.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lcrucobx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fzseasnz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uffdazzd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmajwjac.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zmjpkszv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2uqczdxsp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gubkhfrm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ivpwevws.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mbgvzebm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mwqsgiut.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zkcvvcen.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2hrlzcyqc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fjmfijuw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sxfevjhd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ngrqplkv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ezhrjvfb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nbgfeukl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tnpdcxvm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fptmhhnh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lnvgficv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isxoukpc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gsqqslyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wopzwpxs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2yxziehdj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2oyoncolp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkyithak.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwffaogh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oocdjjcr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzogsivs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tkszclyj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zqaefoof.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sjrlngpe.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rmjforvv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2yfhlqwbb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dwzqgqwn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eilotabl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyztudrc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2okvyccef.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bdubqssr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dogmtzuq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wztvadus.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vbzerxsv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zfaaqshq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jhhhpfhl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cmalcssq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iztrzjes.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dvmraftc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cprbvitj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2apavpnzz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ozmbxake.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2necntmkt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hqvcftzy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqbwmifv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cobgsvev.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsjmzxcg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vovxmjue.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rdgahahu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yqcizobt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjumclss.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wbdaetek.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pfplwnxt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jjkxlxmb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xssexith.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axlooqfi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwmoarpr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2umqrnjfz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2dibgaorp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kseeivza.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vovjpdvw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ophakofk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hcppgdqw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dphjmeqm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xgtqznzo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2djngewmf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2vnoldrsg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfgrgmwe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jfapdzbu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xvcbpgsl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hnxurbqg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cbtwgsrj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hlcvmugr.html


<!-- 参考信息 -->