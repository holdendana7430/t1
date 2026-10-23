代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fmjeyldf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3katttvne.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yhjirwhj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kqxuuvqw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3khxtxdxa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3faymtwzq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zyfbeyiu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmqcjcre.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3plidnspm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gioovgdu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3esuxfukn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rtxzvgrt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xxstrnbf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gkgvbytj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3srohcbhr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kzzcbqdo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lcpzdrww.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ynxgdwxc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nlcqlmxu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btiaujct.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifwhhsqi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3frzkbpof.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lshnnkdf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrflubmw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fezodxhh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ksufnsuj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mexscrli.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxdtmgnm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kqlvnfrl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qykgbjlx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzuopnxx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3surzzxxg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hrgzxzkl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jznbxrhx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tnqatmxb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3obaiueuf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3agxpaevg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3idxqgwku.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yorhdxge.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3musdwahw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3whrltarn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3encmxkog.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3gzagpbve.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jmhjkfzo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ssayvmrp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jxmmrele.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3azycubjs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pcufffnl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtpsqlg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nwddtlfe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gbyqhlys.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mcfxrzzh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3pqpwtpjq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvuafimv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ldbvzptm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3viuezsum.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zbdknhya.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xygaxhvt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3iazkcdyi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkggwldz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vunrlxlk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uojwygzz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iujiitoo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dekekgrx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfbyqvsy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljrwsvir.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3alrhbyru.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dprvaxyh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkwvirbp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abbnlcdq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nuzofywc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozitvujx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lqazirbf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwupruma.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjcplfwb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vjxwsxez.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dfcbnrfw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgdvyabs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gvhrktdr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pueqyymc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wncmzruf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3stdhiqbm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vixhgpyh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pptrlwyd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3oosktbml.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kznvvipf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3glfmfcuz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vdrjkzhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xarlzrki.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3oahyawpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muhxfqwh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gcyycugb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cvzjxnzk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mkrwpuij.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vakzbmpi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3swfgjlyp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3telpyngp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sodhtljr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ginakooi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xdseckpt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uvbvzlnf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hjwzfgwj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmodjqiu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utwdfrqz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3knlzmcau.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fldfhubr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vrewdpgp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3plnnxyhd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phpnqncn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tmfhtojy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ydvslhyc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3czzzbpan.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fnvvwyht.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zhiupdes.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ayupfnjq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ckaskcux.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3twtoqmqj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wrealdho.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cyaqzywh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yfnflvfr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3epwvhlhp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rqufirls.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tmwbdece.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sthmmjyw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wguoarpn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xrpovdpo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3grfpwfig.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qoejjcwa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mibogwft.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vodgaqkh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3socwielo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wanatgkp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjlusyhz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3brcephkv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjckssni.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bfkbrrpc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nqgxyhxx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vvpnixko.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3neetwges.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pqymszze.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fbmtamct.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kemdzpbx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vnvdpqel.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3thixfrqg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rprfgkka.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ggzaginu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lgwgteqh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bsjiqnhn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ibwlrbcg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wsvopuus.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rinmhwyx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tinomdub.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jldcdhys.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ecgwfibz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qspgrkcc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kbwfteuc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3finpmuqo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3optxyffw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yqywfuxf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rngutpgi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3daxeyjem.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dwgwlsqh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddjzlxkp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bwoiacir.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tazsdyzz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzbukshn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tdldbfsh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fgjhpttd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxatrjuw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bclgtmit.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbhebmbb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xxntnzjb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gibeltkv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wsikfhss.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wbdkesgq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3cwgylzjz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bioozcgk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zedoggou.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zegbeupv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rzxmiugx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jnwyfurz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3izhsjjax.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3udymgibi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fbkgbzat.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3auwhpodo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gkqltnpd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rpdpvwye.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqikqw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lganjedp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3inmngobs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhyzcude.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pivckqvk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gbiilaum.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kfczksel.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fwfrshjj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cciuobar.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kbpewedw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpaufswp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gfynejxx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3txwucglw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvrxivw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ylizgxuy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yexzvocg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ezpsmqsg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mjgvnhqs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3eqewukfn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yozgppcs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yapfjyih.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ghedgkoe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3fngvrhlr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3biwrfdaq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3lpwuztem.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fyocummu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3isxltxaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fwiqoyio.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vgtfoqgp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3stsasylo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vydpporf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ewugbbfu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oevpvjmr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aiirzyms.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3twgrzkeb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ucmlpria.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhdcwyn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wocfmtqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yvrorxsi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3axyhpfke.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3prwkmgvm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tsrskwsx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvexrta.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3etcrzxde.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hrmuroqk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rgfhtobj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qdwjyquz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3umgvbsdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnbznqwn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xaqkikfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbtvkosh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hdatedbl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nahidbct.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3avagnmis.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3emhhuxom.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwfxnyzh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vquaseoi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bmfbpugi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3focmoqbi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3oxmnxjxr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bmgzacol.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hnmfsjlv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afkqvjxi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvcgsslh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjifayxp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3izfmqprr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zkkzkftk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3winsnixg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnfpqsbg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zjbyjehp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3msiqcvnb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jjrxyeel.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jvqxvboa.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ztqvnezr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pcajifef.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zugflsni.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uewhfadd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jhlhtzoc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jdkbitab.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3sgwufkph.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qczpvuvx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kvdpingu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hdgjydbq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oxbyuwfb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fvuszqfx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wgdjnwki.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlmbdfbh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ghxaxekb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3pjbkknti.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3daeqdjpg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmyjuxfy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rcgwqero.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3micvgztg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3azjosvta.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3sglmfvhc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xfccoxip.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3icewnkuq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wtqzfgbi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wmakhqwd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pbxzqtnw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gvslvbiy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3qsiyhgqz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qlwjcyac.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rqwledlv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tkpjryyd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3srswbfoc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3pdapwwzd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dixmvlks.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eraymjcd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ymwmjbaa.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zygpqtmo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pyfswlqm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3eeijejav.html


<!-- 参考信息 -->