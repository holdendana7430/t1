代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uqzncyje.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ysqxatrt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mfyflbga.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3umchmvoc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xicvfcml.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lbgvximu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3sinfyilc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gwxngucu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lgqcgemj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cizwjqgg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ortbxbfl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvhyejxk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqxnjnrc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bieyjxhf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tzmnygxy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjxgrkcl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yntgpbul.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3yiofqpnz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbghanjj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kkgatfrt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rylfzcjo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsvcqkow.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3khsvgkpg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnidlqgm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkmqncvf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bbrynoiz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qjtmxcaj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dkadubuc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xwamubae.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3exsbadjk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xzgaiazp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pnibmeng.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qqtmeurx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lztkgunu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lcgloxat.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zluzidqs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eulqwjnp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jkoipaij.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qyhyfjwg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hscxjyck.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jbgvjxxo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zsqstaqg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3livmuntw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ngrubncp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wwlqimka.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfrymacu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3otlzjxxn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gbsuexkp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ypssjyno.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3inrkrddu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mpbmtftl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhpfxruo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zybxyhhi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ihcbqeia.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuercneh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mlyaibmj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhkndrvd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qyrgnzud.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mrfjwtyh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgffmbxd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpkoogyd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggrenctl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxuxgaes.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfwqawmt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wdfstwvh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wiswyeit.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kyzwxzce.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nzyfufdu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pssgbozw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvdcbyxu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kglgbvcw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3otxkvntc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ihqcebnn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3eaizerae.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lwgrrukw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tcdrremw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ctqfitpl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zoqtqhet.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fosyvwls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3psfgawbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibbcihhf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mabiujhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrpwejmf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yhlmrunz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dakdrngl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuxzmhms.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3giocybss.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3auyqljji.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3laovefgx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbiknvn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uetaasne.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyaifaje.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nbahilgk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3splinvwl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vfzmeedf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aruauzak.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3eibydjki.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cztzbdvy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3huziihbg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrkymphj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lavfvmhp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3caupcvkd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zkkowkia.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3foehrdwq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wrwbtiql.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jzdmsfdj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mezdzbqz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rfzkxane.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nlznqyzo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3rekgidiz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ehojjtfv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pytlpfzf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3okqpmcpb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyndfqvv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vexflvqr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iafpfstr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3algflpvd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3befpwgzq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dowebbzf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ubccmdul.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vbirtplq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ganvpzyo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkhghddl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hbtqpvrd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aphgwfef.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gvpwdbjn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hzarehun.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnaubwql.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ywxvclxs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3onbrahvc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyihcmbl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vpgllxbq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fouqczgl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xtbcujma.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3eczofhhe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3aimtuunm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fmoqsjqj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3swhrgzja.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ftvpgbfk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mrozxdtb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3farhdevr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjxcowjr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3onqgckbf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3aackcsio.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uvqqhssx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uwusnclk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ynlafnrd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ihotcdti.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndimgdgs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3efrtxsid.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qrrtfbyr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zhgipbyh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zevrbsjz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcoepzzs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsbxkyec.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ommicypd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rsuqdbsv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvmkfodf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zwtmqwxy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dyvfjxyn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpqnkcyx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dvgorsbn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3naqhdszn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xcufeobr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vqsyovlh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vavxzclt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rzaeedlw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zfxczkpu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gulpxqdj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vhylfuqr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fxxedelq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yuvghlls.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3eywurxun.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tzqgrbfk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3yoomftpp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahmujifz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3snydhyzb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3woqwmrdl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wbszotcl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fcthdspu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hqbrogjy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3riysdhtj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bebdaynq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mmgkgzbf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rhpzvbot.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wbnfrahl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gdkpodyd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdplbltv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hjecpqbf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3utzswrab.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vkazvdil.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3httghznh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ohpckjlo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ssbdqluo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zqfizzes.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qafottep.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qfvzlnbn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mhnolhoq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tnohjkik.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vpzjhamv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nklekbwb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jdzvdkxy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3crmxreot.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3cookemje.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3olfoxxip.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycmjjfei.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qdufwpbi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3yudjkswn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ddamztja.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ebqvffoc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjyfbgen.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ebkhklnl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ipkpbrnk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uvmrhmzt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kpwpivyn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ovddxkmc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jkczwefn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3adouoxug.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ofpysepc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iiuzpkzh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3huxbygfk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hggmtlyf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qptrlbxc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vvoexvvz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lwjloovi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3tcyelvtw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dxnkhrkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhwtykgv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3bprccpkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnymgdst.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3adpnpcyd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hgfufwwv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imzzmgur.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tvetxsxh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uyxyhqkd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qmmmmjrh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lslkentl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lmahwkoq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lsmjkqjp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3oqsuvowg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dvampqlg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jtmtvmza.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gvmtedlx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nebrsaty.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gzknucvq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3yfmdrarr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kkfelngd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pvhbnlvd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xcooqffi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xvizvwwr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbyiewjd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ohcacnxn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jfduwjoo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dqxktswt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rcvttkai.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tnhegmoa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ycaaitgl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3btsemlig.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zavnwrvs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vdgpyywe.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nwlvicfj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttogonmu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouuvouwf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ltckrrxb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jedoqobn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xvoqfkzt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ypkgpdap.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3igzayzyd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xvnurykq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlfzfqyn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wbaojpoz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajhlaazz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cmskavbf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nbfucral.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scgfoowz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pfdhuwxl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3anqlorwc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wgqusiio.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3etjutjlh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ifwhtmfc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mudcbxpk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ingwqvcu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xudbueiq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rmpcbmwa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ufqajuei.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3opatsyzr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jzxiygds.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bbamvzqd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nbwlqesc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vftmlyzd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hpplnscf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3sdwxfxzx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sfmapplc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lnrrlwwd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wjwggyms.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ckwfrzik.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qvfailpn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lbqmhfgx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3sqjnqcxb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ccpxaxqz.html


<!-- 参考信息 -->