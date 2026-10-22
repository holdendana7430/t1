代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vbpwpdnr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2azulyjjm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2raoswsah.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2cpgkcike.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ncfhadri.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jfaccrdt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2brnydxwl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dhkurxoc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2awblhjeg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uauceutq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gvltcfxp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sdpgzwmm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vicpqnmq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2domcsujs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ubydtavl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2smsfoker.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xbtqzlkc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ntfkvhju.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ghjrrvht.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2swuiyhbf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jddxmuvl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2aoajjvkx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2shqdcdeu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxxafrey.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcknnzxn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yrgqrggu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qysmoaxm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvxzqajn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxfoycee.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2txcxezqf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzcnqabm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2azrpsfuk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqhudsqq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqfmooyw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2odiqfssb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edlfuvzd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfnqrnld.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lgfprkff.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2syrkssmg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lkftazjj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jfqnpztd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vdtgjtyl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dzmwkbeo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jxotidmu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2oxamlcxs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bixhqsan.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ncasnpue.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wbtlmkrp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2behhvoqm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilgatjkz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2atcddyhv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nwixtesb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cfbjrpcd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lofbscko.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gadrebie.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ahcfhlqg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lswiywii.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzhagaen.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2scvjepgn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xfvripyy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ozvxphhv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2afnohxbk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hbrbgegu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syvgrlki.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2anczmzjj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ngklgyiu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nlfxrpll.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2onqrxlys.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zztoxdhj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owestyfl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kfyklnvy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dojmbijf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gokygcbh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffafvvin.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fiaiiopr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpoikqmh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vqxwvivi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2onolmvtq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxwsgjfq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oywthknj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kklrfpxj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzaujths.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nrpmrluc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kglyoncu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vykrseis.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2luacpyne.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ilqmuqam.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yxawazbv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bnkynxwe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2epzwdtzd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2bcswwbaq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2iljsydcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqtrhscl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dszzzeoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpvemzhc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xhsvzzbp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vsxejfje.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rgrihgic.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aulwsnra.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vgffmvyd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tmzxruct.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hkfxtton.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mznbkmja.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mrmolfmu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uijiyuzn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hirfbqkh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcqvzhgq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zjzmbfei.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2batidtbw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kvjixaha.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2afvzfdpu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qvrwnnmm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vyqujsja.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vfywsype.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2umxyeoip.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ztnucnjx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jqoqhuye.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nembifvg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wjnfqcak.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fisbthkd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gztxwxqq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zgwskgrz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mazhtzmn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vyocqrst.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzfbpvhi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2marbvsuy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoxscxrz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ylysjtmw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uzyqyuod.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2feyokgkb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tuvccbus.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qzxtlbjy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2puojoqha.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vomcafcp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdtuuqbj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xixjvkzk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aslkjkuc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rhymlmip.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zoacenbq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ckkwgexy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mslfproe.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2oendejaz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2waivxuhj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgaorcgv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2adpqgkfc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chsbdpsq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yykhcxra.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xherygop.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xdznsbve.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ykjeayvq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fjxislyl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2oaiswmaj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ylxduuko.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iyrxtuol.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fwxpvgsf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dambopuz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tmzzgjmt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zkgitosl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pqjhqvme.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qxpzeowq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rrpefylq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ftxjuptx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hmtuxyin.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2djdlqmzj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lvdcngth.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ngbykvht.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkhfmmvl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fakpozor.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ywlnlhei.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmcpdadr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ndbkqrzy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2irqhcqmj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2smqttjwx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xjtrduxb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ipkrmkwo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yfnnsgjy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gusgqybi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ipopdtpl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pbnvmmvf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rvodnsne.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pdvenfdw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jgjxoaey.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jngnvmon.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vaqjwbng.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jhcaaksn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vhmnzfnx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vlxmlvov.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lalwnqac.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2keidvhch.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryfsugpt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wgevamtg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qywudayx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2owvzgbes.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dyanzgwd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2loqnqawo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ppdguzkm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2syaskatf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzzwonpg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mtamqlro.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwzivaul.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zachbgbj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2swfzeayk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2izdvkkru.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ollwspbg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2klpdscih.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wqrokyou.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bnnxvqya.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ttcapiss.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hrpsqvhf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2exevfmze.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ergvxphm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hixayjyd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rwyuwbiu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zlszjmzi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xskeumrd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2gyngjgtl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kilhzfza.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnrsleog.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2asdbcgqj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2srwlwjrr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dxfvlraz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qwgpavki.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ctzpspuk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2csdimdrq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mrgfmwxu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kgdofjvh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ddzoxsuc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nrncbvvn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2usqlnczj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wifbogfg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2pylbagxa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vpgtrruf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2helkrcgd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nvaokrad.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nrmzpeuv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qvnoqgqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gmkrnhfu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tcscossw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ruqgslms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sttitvkd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2tfoulqfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2heamljoi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kqrysxau.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tyzgdexs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pfmmtmhy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2farzrxij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cwdxkzwu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2aupwhojf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ieazyiqd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2anoqcuob.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeapdmgl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ouuumbbt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cgtywqkv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2owvdqqpa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ilubxohl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqybsdmh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wsjqlvyg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2tstqjjnk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zcjmmskz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oovtemtd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fcawtovi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zgmvmxyf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tfzylvgo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jummrjxh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2adlukbgg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2diodzbpn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vxqjxlaf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hlmkclgt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aryokkrl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vqehfjlc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bjkogfdo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qrpwqwps.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lexuadxq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2epvdcviv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2umzlrshl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wxgwjybj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bnsrtqfv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxccthsx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmkwxayb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2jxuvginv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xlapkwyz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hxystomw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpmqdiwk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cjggacaw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qbvulzxv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2naxraebk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omluuahr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tkplzljk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vdbzzqmq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yulcjoxf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lviaeckl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hzhnqxni.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xuthpaen.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2uzyjbtpn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2grmzvzzy.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2txpyluue.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xcvedjzi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xuepfmbq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hvkbroks.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pmozqwdf.html


<!-- 参考信息 -->