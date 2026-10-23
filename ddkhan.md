代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vhomrnrb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ygfybbqo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vzvhvmgs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3foydkpez.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uymakuhp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zrcrpiiq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wjqwfzrw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ywwiqbqz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zwbdaayu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3izgkvfyt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cwxwilmk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vvrsxbxn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bzqdbrkp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3miblxpsf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdsehbgz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfvxmsop.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhmqkpvw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yjbeyygf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3julxmtji.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptopbmwf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qizkousw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3shwrwiqu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwbvkttn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fuznrtqf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcuhfjgs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zihueamv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yryunkil.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaqnrsbz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rhehdylo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3afrmopdo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lvyonpcp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zidlqrso.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nemfpihg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yhwqtdxj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kivgsekv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hiktlywq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcsjeyk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vfxouzza.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dzpnlhhu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bghjyzhr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkiymit.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yrhrtmmw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3aokilzqv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uhmlgala.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uqtrgegm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qsouqrvz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tomhchsp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3eyyltepa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ayocuvtw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfocljjo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tvgzyhnq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3afgegstc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3snstavcw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gdxhjxqu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kqncrjcr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzorjoar.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hlxdurmj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ctjmigwm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjcswhyw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ssseubwc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewmgrlbk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzxhloob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mnsvsyad.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvlflexi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpoaxdzn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eppybjmb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqrswvne.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3naxvbbbu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3leqcepfk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xijbifae.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugzzuowp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vmhudzjc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yrtxlzij.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivtwttzg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3livcibed.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xgjanmyz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3usdsyztw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3grboqham.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lqoiphec.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3iubrlpak.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3fkcrsrwz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zamqtofg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3asjikavu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3oqgjgzlp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwchyhie.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mzluackk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eampxgwr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lpwycqqz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wdnkznpb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcqkwjzy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tzbhyhby.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xislnmss.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3krldbvpl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hxtkjfdw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3owcywebc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gyvdxukw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mevcaqbz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ysiffqof.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubkoiuon.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nensenbv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yahlykng.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgcxksgy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nplfptwd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nplwkyjo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsoedgka.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zlhtouig.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zfnrwrgs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3usagvjwe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zijjgcgq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wzvnoqfv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rsawkwcj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nspggpmb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3icbqxgrf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xyitraps.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3szdnqxvh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ktvurdra.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgecsfyr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ynutqcqx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3abxkmiuj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zkmchuwh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lgfbkvym.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3miiznkpr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gqbdqokr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nybddztt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3igwqvytd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xxkhpgxx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qgevmnui.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sctbpmno.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwxhoact.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3uzdfdvmb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rtvgajxm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iskgbfee.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bjykwqvk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kwrbcueu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aojmzzot.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3omotxksi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oewdhmvy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3urdvwuez.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3aoeycnna.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ufcuvjhv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wyxciyfu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3osopkiec.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jhaudhqg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xqgfpqcw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hwhzbkkb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fcmkhwlz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uyepxhaz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3amzhojmh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3oeiemrva.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wwxuxxpl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3sivpgdia.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nfhvcgoo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3varjcubc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrmskjtg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3linovmjy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ijavlvuu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cnoejzlg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3skkcegpe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mwxhlvpz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dvenqceb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ctgfpnyh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rjwtxdkg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ymmubndy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxzqjkgv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3teizwiux.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wlkwvlry.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yrsmphki.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nhjxwhmt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3eunpdmno.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ctsvbbsi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yrfvdqxh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cszqmuru.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3azxgitsh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hiszazum.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3prcsqhrz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vqrjztel.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fpkwwawi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zlozwzwm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dbznycgy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lstakxqy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bletwlll.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qtyemiev.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vxudqazd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3omglomfv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vkzdvcsg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mmfrnqmz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ulraudfn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tmifmayg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmhhwssn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tabhrude.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzcirabd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xqtykmsj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rbvwhrgn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mcmtfvxf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ptfuakvn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhbqkjpj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ksoakftl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jhvusgyt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ynmqciox.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ieoabdvm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iyljgliz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3eqbemymt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kohlbijz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mtegjxyg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ybxwzzjp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3irqvdcpd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3igdjjipw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nfbnfdom.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3igvlbftw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mywkjdwx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fheedlzf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fatsflpq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3izljaplo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ootmbgsv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzjtguxf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwwdfnfc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aesjcrtw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pbidxebk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zvkhajrg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nmlbdzlk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nezuhhqq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qzarapnu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nwhtttqr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ukbkxixz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gcuhbmzm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rvhfkgir.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3emeedtvc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3igqknbxk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hbybchwm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3uapskyxh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uxnhtzpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okbvifhq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vblldtbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwlwogka.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hiwpdxcy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3icsabugx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uejoomnt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ofqqjuew.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xlouvpow.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3szjzsepl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3habmpjhp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3toacukqy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xgnapbep.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rpvongfw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3iaymtduq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eltfvsoz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evrayarz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wqwmrhbv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bshoxxdj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zaywuvgj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxwqqwgx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tdzglpzn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xqzhhxfd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ibwmnqub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3shlyzaxk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tayminpb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xsygynel.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bikcfqqf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rmnqcdss.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ivrtrcbl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3myqzxayv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jnkvylme.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3quzzvrmr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fatbqcvp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnzwvorh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pkpbfsqv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ijlhhdpy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3huwvrehx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbsbuqlv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3koqnwwui.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rcffgoux.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wmzvfmwv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hqnwtfas.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhqghxjc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehqsffuj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3xgfwvzdu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmnsyxn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3azhsczor.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ljgcavul.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uxefwpdh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jjiatofb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qtrcityz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xpfxycup.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hahmwjyk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3pxazidxb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3emucqmqh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xucmffon.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bxkpkyla.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nplkhopd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qgjrygbi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fdxasjyu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3irccouif.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oihsquhr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3sizocxnt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ctelnuxc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gwweiqud.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lfsfqlpv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3oustvfrh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xffichyw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jkbvtrli.html


<!-- 参考信息 -->