代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ptuxqmfu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3acvimhrw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mykvmnpu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtnedxto.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tdkntqwx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pfvlsztj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xmpemurs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sddbdapg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gchqsmpz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lijojksq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dqyafirc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3khyqbrkx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rctocvrs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pjowzwmw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjpkthxm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbuchjup.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmoqadyo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mrmydwdg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nifheyal.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urnqaucm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eazkmzfn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dtdkaber.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpbdfrvx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jslxhsww.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuxbyhze.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlpcsslx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3djikhjaw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzgkkgzq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkiibvcv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fkbarcrn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3aiiirxpu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bqtxwuir.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3chimxnqw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vbacozoj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xnnxpser.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xzmbmfzs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fcwmsmaz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3znnwkfyw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cvmhavss.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lbgkgaco.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hdbksdeo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgueyjpb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ujvgigwq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3acplziee.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ovolkucx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qrlmwufy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3utmwtiub.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lnvdsorn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zowvepcn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckdvtomc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fpgmlezj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mxugbksq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ssasemne.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zziymqcd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zvvhaczp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgdjdxhx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3klngszni.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nddgemxb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhrdzzvh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nveqcpxi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iilcvusm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dldrdtsa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vbjtowsq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfatjtxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvakbdje.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sulqqcvj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3rchswyas.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwlzlsjw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3buazfndk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxjmdwen.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgiofsiy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vflbqufv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gfcphmja.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bsrommgu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sbabetyo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tnpseqml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3invskjiy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ejtchdll.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xbnxgvur.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3irfpandt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3okzowgoz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3luyaxwmw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tvlrbrjw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ulkltblv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnvvxcrx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zjfpmqfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khajevmb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ebhyasno.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mfkiouod.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxxznznn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3npchmpyj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhakdgvz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jwggxfck.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zjrhcylx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bliddrkm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qljqfcyd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3huuqchzt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kkomkzee.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3minxfraz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uleklimv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkrnbnlu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvbzdsqp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3iiavxchx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cvdnwwaj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdwchlp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tlwlurqi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tqteekyi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gstpsaxr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oglmdjjr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aijdotph.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3txemyxjl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uomvxspz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fbnxjwnm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3kceamutg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3panwyatb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qmqgvopd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3djzmbpuv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yghwycao.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bexlzfsm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stknuemp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3prhnphmf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nsgeqmna.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dfjclatf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tiptenip.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zhbnorgb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyhxpylj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaseyolv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvyvjrti.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpxklnzn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3itrcosvr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3leyaeelw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ysdiqgwr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qrmqtdoy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3dzhrjxcu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajvhomex.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3neppuegj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3minwgfxm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wxohmyua.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3tyjbrdjc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qnfozjkz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pakwpndm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dkbkjdzb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ntjoqdvx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3djoemskx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bctvpbsn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iurqpasi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cwqaputu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3apkhqwqz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qrzfdhuy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vianapfc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3awcfkjpg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ccovppdk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vaaaykml.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccyljrwk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3odeomegu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ubddwbvh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jsmhhrxm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wjnsslqn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xusfbnsa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qzwrmgqp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3amtkazhj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gzouavis.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kmzcrxzl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rvocxzhe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jnvaudxp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qexnyekc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3czkpmwrb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3jchfkhjm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dybpnjts.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3dvieytmw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ipvejgme.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3srvdvpci.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uwyeiigx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3diylrjit.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3djvoxoky.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rwkwohyw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jnxzezih.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xuanlatb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wlyjhvpz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pgntlnol.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3azwhtitc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wjdfgbbv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ccymnjgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kidcsuiz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qlchytfr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xgwfjjbj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mdiwqwgq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gnornaim.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfxdgpvu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejuviwnn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kabincxj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xwhxwhuc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iunngbsr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tvbijqcz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oxuvjqgd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hsojnzcs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cszqmvkc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hreirlrv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3emzhawhb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3acvcmgke.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3axfbggmf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ytgigzul.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3psvvlvqt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nsylwxuw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3anxhcmnk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3lbqmyooz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rgfsacga.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xpagnght.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nzhkrdih.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eypdkljj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mexcnxpe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3llbwhbjk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kdzlnxrd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cmnvyhon.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vforbnfi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltyqhpzg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3uztzwzty.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3icilyysh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lavfdquk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tspzcfif.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nukqpvxv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3njafaewr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yevjcdrj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wrzeddiy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gdkceqxv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdvldphe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3unaeudyv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wffoaska.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3nraksfii.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ophjtdpx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ucfnsjbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acywvndm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jawngsrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrjcaaee.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dhxggpul.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rvmixnvg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoxyzihv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdxwcica.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qpagdasu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqnsqaoj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3skxpqheh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwqvzzlh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntfbndxv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ytntnvtx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cecolmwv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3btpnvspd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eopfmkoc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jtrvhliv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojgwwjwt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vielpoym.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3plrpmmid.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3khpmxucd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gllqjvlt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zqgnrozt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wqtpqstd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iyfgxwwl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3prxsgquy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cfakcpqm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hnoyicdv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3owevibia.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3elxfyrvt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dxuzqdxl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mwzvqjuj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3indpbuut.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvmswkpu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ritrxdce.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uitgkild.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qonkqpiq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffiphzig.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fkepseds.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3saeauwet.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3izhpxopf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cgshrrbo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftixvmff.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xhpmoauy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkeopzmz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lssmayky.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dedetmzr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrscswtf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vnjjpbgq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qkadmxlz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3huanopny.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3evdsqotw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uzeentrs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3glcrcnlc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ahstlozw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3eielkzdb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kowbqtrx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jdhizjgg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3quiuhhvu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pgdycyoo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3giokbwxs.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3glirukka.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wgvziuab.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hmfsxizz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vnvccnrb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fmclnkbw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3iajwycmi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kkwlkdcx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mdelkyoa.html


<!-- 参考信息 -->