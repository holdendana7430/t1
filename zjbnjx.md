代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wyemlgzn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3erkduase.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fmyxspfy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yhxjsimb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gvirwtwc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xkiqgqhs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tvfryggb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eobtodzv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3miyonjfy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vkxszbew.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dinwvdlg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zeoyshmv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ottrtgkg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zzujcenx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rvspcqmj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3puopfvyo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzaappmx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3grgffrvr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwjuxarh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdavoigt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3compmvjv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqpppzah.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3chlpyord.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qslagcpd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxyrobpe.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mgerqxau.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ubojxnls.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcrwnqe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3aianzaxp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eopuvffu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wknbihue.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3eyjkvevi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3iotubelt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mznnqzli.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vmptmibs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zcznqpvf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lvhnqxym.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofrcaznh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3osogfakx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3byktcxrm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3eifomeus.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bmluagxe.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghsrcgkx.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vzctmiwt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ceseuikp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvrqbqqy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oxctwgdl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yfrqvaqd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yzxkcmgs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbvzwmty.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zladvubg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdyfpdka.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zbgrqnub.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sykpwefn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwbttidf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ywabldgp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lslqmxvg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vpyogjkq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ktgcaizg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqnqgset.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dclcqhnr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mstqyakn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qtgtcatn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exovltno.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fuecqieb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3svbipacz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yahltfyl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3trukxhxc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qehwlwcm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxuddaoa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ujgsquja.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mkjqnimp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwmqwzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hiqbofxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3oyewxoro.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3awarbowg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3quunlezp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3aqridluk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yazucnhg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vcowacgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgiiaean.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jvybqyzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huedrzle.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pzpyapap.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3idmvmyee.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kydqhull.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxdibnkr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbjmmxyy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fejnkzos.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3tkimsgrs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kqrndner.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hplhuorw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nkjadaxb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ahekaqvg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfjlmctt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iggsbztr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vfhvmrxd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ftlazckd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xrlybome.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3sfeyezba.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tawrkdib.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gcdolffg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mdgqsawo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vaysggiv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dtklsovi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nhxffwro.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3eaglppiw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rddvfrdx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3imptddtg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jsebpbch.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cpbmcvjr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3utqiuqzq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynulqasl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgktsxaf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtvduvzc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uymaypfb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iqatnjxb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3oiuffiwu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wuaqbuha.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rwnzhlyy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ikvwtclu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yybfkpgx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yalrijyp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ytlmfimm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsgsabcz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yrtrkrpx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbfvbcbe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3epdlbtuy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3loohnjqy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ahlgqmws.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iscorxvh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzvbmqsl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3anhhsmcd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvswuuk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zotitppv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lpkokzwm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cdyjlnbf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ibdoibvn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zjjrxdah.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wvquuxue.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mdthpngj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3agtvqzej.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tkakcfru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dhltzfpk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wtvlfrod.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uihxmgdv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yyqlcelh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dpmoaqyy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3paqugesv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3smqubhmr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3adlefjky.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3thapelkq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ktbcbrqe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hqivzmhl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yifxzehe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zosmqtxv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3phktsfgi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jyydsnqa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gxphskdv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fhlhooea.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3urpwjoyv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vzqkiboz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xpqfjoem.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vbdlcjlh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3eolarmaq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jsfwchst.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vpfizdpz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kxysaevf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pkihbzlv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nstwijkq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pezljrhk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bwkujrhi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ojdcmvhs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gsacghnu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hiiklqpw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqjccxcc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fygcynqq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ocizbcni.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mijukjpu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eokdzmij.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wcapwdmf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3odmqcqiy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqcbouus.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hcdzqcis.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3itfddyaf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nlfznsnm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufjvklpd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uzhyujov.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fezfjwqf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wggngqnt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lbngefgr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pknadwig.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hjcsxylq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tbrtnzqh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nudfjxwx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ugvbppaj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ofmuivtp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vlfkxrkf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdhpvje.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zoywbikq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vcwkknfv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ozkeiitw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3buxnlftv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tjlcknqb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qjxuzzri.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vucfnbnu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wtlynlsn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vxuajasj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lxpgcyow.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jxrjfian.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3oeyksvje.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rqmliidc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ocpjiagt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hhdpzbey.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rmnkynkl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gooivnah.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hlptmftd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lgamscfp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ljqxlnpx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3awbplzje.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vhbrbkik.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3oaxtlnox.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sretvteq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mdkwpkhu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vczywzjn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3noieueck.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hblfrdxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjkvgbiw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ejuctbri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bmmitwmi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3edyjwnma.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vnclrwpo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zoenieuk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mirwfycy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uihafutc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hzoefilw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3iuiejxdm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fetydwpp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3cyjzhnzx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kgginjhw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wwzggonb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3frihotay.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxuiugp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tvlfxluk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gkogguob.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3icnombyy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pjfamqtj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eygmzuvc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uklwdrad.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fnxahhis.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3milkzowh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vctgdgny.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lntvsxmo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3olqlshsn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wmljrtpv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kmneozuv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3esqngejv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3wpptngnk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bnwhyvsr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uvedsbiw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cnmdrzvs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyomgvsy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztkguekl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3kuxarqek.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vcvviqeh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3moburgqy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3myxlnezl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gwyvghvr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wxnecddb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kicszobd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ssykeccv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lokjjswr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3kzvzhggq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3izwifnek.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwxuomqc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pbiqrlkr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3yvqbunry.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pnkawyfj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qvyipujm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3seufjwya.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ofmgbvdp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3gjidzjhn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rojhcayt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rakwtsww.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3bqqftvff.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lwyazlgr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rotafock.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kvieyrjn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cbandevg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3bkwdtque.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mkvoefhr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qkbmqgpf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qwycusjt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3bjvhzyjs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cmfzwkzk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3nufabids.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kupviqad.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkuzkws.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mrcrrwbw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rpeyuhpt.html


<!-- 参考信息 -->