代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gvoavqmlq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gnlwpwfqk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/geuatqtjh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gjsziplgn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gwlnxjehy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gsmeagrjd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gibentwxh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gvbjrbvjk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvxjkpp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gfymriysh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/giycdciue.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvayfhphc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghjwzddkg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvatgrbau.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gvmunrzqv.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjkxkqjne.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/grpfxcqcs.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gxkoqzitv.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnkvsnlwg.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtpjdegek.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/goviqqici.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghcglpxla.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gtszwjvjs.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfwihdaat.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkzcknqcw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gztucxrdb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gwfzjheit.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gfwiclbpp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/ghxlhqixg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gstinsdmy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gqjhjvoyn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gegbuqqww.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gicgltdhc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gipypdmmu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gvunrsmkp.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gwbsyaeco.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gaijqscgs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gsvueothu.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gmcasjcsi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/giajbsvjc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gkodfscdu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gwvaoampn.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/giffmgyqw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gcpfotmpb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/ghipbulgv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbhevfnio.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfnpopytd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gkjxubnfm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gtsjtilnd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gctqjfhkt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gkaliwujf.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gueqddyhu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gnucxwprj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gjexgyfvb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpamhqkcv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gilrgzxlp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpzmclfvx.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcxjpsygr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gsgsyrnfd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpcfqjshl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gienkyyht.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqfhtdutp.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gukqfeuqp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gxwlzoihy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/getjpsobr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkfmbdlmn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gebnunrls.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdrzpvdvt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gkkznbced.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gjbldvvql.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gmnlygswn.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gvvnwmthk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gzurkwngf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gsvwnixfg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/goioymsce.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gecuxqsgr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/ghryfjyjv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gfdbibowp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gmzcmqxgf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gqdzvfgpl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gugunfvve.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gvsrymiuf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gymwcxeao.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gkztrskux.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gsemgptyo.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgjanff.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gmvjfruzd.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gqtiqseix.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gtobalcht.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gyyhpnrts.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gxvfkfryr.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gljivgdqp.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/glkpxmyuf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gfinjlprx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqdsmtzdb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gtxfmdwqk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdgejfcwv.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ghnqanacv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gnqzzqnaz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/grlxmqvdc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gazxulmwt.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gqjujhdmv.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gdhvnbkoi.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwpervtcx.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gooefmamv.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/ghnyxfmhu.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/goaytxhwo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gflqwrggc.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gjkmwdpsz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghjcmzwqe.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gcoynrlha.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gxhhfczzk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gukdvwhus.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gavtuxrmr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/grkspgoll.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ghwlnmvjh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcxkwrwml.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gsughoiux.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ggvknrtxw.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/goperugpf.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gsepgjray.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkgnjieyq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gykkidqnq.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gsdizdkkx.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxirmccov.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gixzdyuzo.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/grskolhgj.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gfuwqaiyp.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gpvraodyl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gyzwsakvl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gecdnsxcc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnfotehot.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gtlninltc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gaocxlyst.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/guybcqkls.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gjfgfksuv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/glfrwpdwl.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gerrwixto.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/ghfcirwvc.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gpyzqmnlj.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/grfyzvjjd.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gqerumfsq.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gzxjiglcw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gvnfjxnpu.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gulrexexj.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gfxcljbuq.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/geabghjwv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/guktjpdjk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gazjipbzz.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gvkdjjdry.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gvfzjcgdj.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/glvkvqsma.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gzybgxvpk.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/guyotjjuo.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gkplenjlk.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gokaxwbko.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gbkduiuqu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gugiqypsx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gygtmjzji.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gqytnftal.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gzzfwyitw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gslyyekjo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gmfftuukm.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gsjlrhhxj.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gewyoyhnt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gkqhuvsvn.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/guflqmcdu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gqdfpgebc.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/goxteqmdg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gknqzafgs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gfcbtjkox.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gcxadvjnh.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gbqvbvnmy.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gjpfufrbn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gatyxgpzo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glbtxpkrs.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gezrzezev.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gwscpscjr.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gwdmhguez.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpdvryul.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gepsvgcip.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gtzqjrrbd.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/goydohttq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gzqdgydqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gttzcxinu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gosuyjlhw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gyyqmvhwd.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfnkqtvnh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gnnivhend.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gsmzpjozf.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gsfqkggzk.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/glayioprr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gqxpowptd.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtnifykeq.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gdccxtyvg.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvmkjsvcl.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ghcusomsk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gdcxfadea.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/ghkjdwfxy.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gwjfaanxk.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gquctyhjy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gjzwunrhi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gzgytigzy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gbumawxai.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/glqtqnpch.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gysivjnoh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gubbkapdp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gphgbemst.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gsxcmrqto.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gfcwgkjwt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gnoegzmca.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gjvgalmpr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gufilqjmn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gerssjzqg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gbxklsssw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gcaytyuzl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gqloonrff.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gfunviwbw.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gfooosbgy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gpdnxthqu.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gatyzlluv.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gppeqxkli.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gidkswzgr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gcfkfjhns.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gboyvwjwr.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gzlvhadnw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gvayziodx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gobqkqytt.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gyujnsrag.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggppczldt.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gruityfif.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gubsgoqcw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gaqdjmfzq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gvrtprvus.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gehyvkdxg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gomifpurw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gntcekvfw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gvqoiepek.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gnrhvofyt.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gbfbuaesx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gkqtpviqy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxissghga.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gnyypbgrq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gldicndto.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gkerhgqij.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/goqvijazp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/ghpvkaucb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/glfsdseed.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gzwoalnhp.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gdgxtxhmt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gmrbltoyo.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtzweiomk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gnzvqlfog.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggschktgs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gaabmxdid.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gcrxazvgc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbbyfaeir.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gimqmcxgc.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gbhmpmyvg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmovalfez.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gsjwgdkiu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjunpayku.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gqcmhhnbo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/glwbbsftp.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gpktvnsux.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gvunnllxo.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/guarolbgn.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/goltcmshs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gsgvoeuny.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gkdskdmim.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gxiwxeidh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gtaaxhurd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/ggpkjkomh.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gwzujhaqr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gjbqxcwpp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/guxvowlme.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gqdaxkefh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/guzmgcpvv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gjpyiagdq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gyozdcbgs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gsscteiqa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gzwkjujmd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gxndaodlm.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gygyojobn.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gsbbxubut.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gflovlioc.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/grtkxbzgv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gkvkuxsmp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ggrwewomn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/ggcuvhjiz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gxogsahjn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gezqserbr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gnbolckue.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gglrdomhy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gsbkfnfrl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gwscgzvkg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gbummgidh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhwoikd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gbtculgsc.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gndslbvmz.sHtML


<!-- 参考信息 -->