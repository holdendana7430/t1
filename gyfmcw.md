代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rmilimnu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zsorjyty.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jjnxcpbt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kesxvznx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bmvkewhw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2luicahhz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qloqphay.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2aiulersx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vveihich.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gqjaurco.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ubjxfjyi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dinumzxa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2pemcdpzs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uzvjzmpj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kilomfbi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbdusdof.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srxsnmoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mdivwwrn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nqpuncca.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aszsofub.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvgrgisg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2okblirgr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vakgcjnj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2amgystax.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fehqkjig.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kguorsom.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qlfppdyl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovjlxpek.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqctzjtx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bumwsbyn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mkngishs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnrzfko.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dngxjxtv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ugrsbkmx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ikipalhu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pdlmburz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pzujcqix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cvzhemoa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2iojqslzr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2puqcpkye.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nqocvrdv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rdmjhlqn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zocuczjj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lbwssioy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmvxdvx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eucmfrxh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2evsezqja.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zgxdafpz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2anvjyhxk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qtfvmwhr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bnnztsrx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2knwzvmkq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ympbgttn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fzbxojar.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mmvoadby.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2egauvcgu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pyxzywkr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ssjcmzro.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foqzspcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jempxoav.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wluvecpp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpyofdvy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kypuobbv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qiwyskau.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyzhhudn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtskrxpc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ostkqrxm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgenywek.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dauznwpg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pydnbhdx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stvfoxim.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ysnqbkrn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ndqngagh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2guuxwhxc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2yxozirjt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ctcaoopd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2uchjezqe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wfularse.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2eryhlszb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ghwmyksa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tpfzazfu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ietglews.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2kffpsxrd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kkoejmyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvgmskza.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xvbfzdsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xepdwcdn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lnznenpu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2koxirsju.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltmyolbc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmdypqfl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifppzbax.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2juhvykzb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nmiehsah.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gmtjlwks.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjmxvzwm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pqyyuqcy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2irtgwszt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbbmxcow.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xajyzogv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecyildgm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ybcedhxu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvrtcvt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffkfvndj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2przzqyil.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ygwqmuax.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zdntwuhs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eudxnats.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wyfhlkol.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xnurmiac.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2urabdqwo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pvknkwnq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hkbwbspm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2foafcbeo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rjaenjsy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iltjdhne.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnivwmos.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izcggjjc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxogovcb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fyibenlu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rnosqlah.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2awuqxumu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nalvypqi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2grodttsu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eqfewzgq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zoipnuyx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mpguxzkq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ezxludjx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fqrjdycu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wcmytxrz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wzjtoemc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2owkavgtx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wuxarvhe.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bueanwrv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnvhithl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkhiexno.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzumqoyo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfpofhkk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2joflhgpc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dyxgorpq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gklajlaa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qnhkuyxa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2njyhybrp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2eiauydge.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2olfvivbr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ceapfcot.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nwzasnok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ilkrhkie.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gikcswkz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jdrlakzc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2oqqyoyby.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hyrkqafh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2chjfgdel.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ekquhrtg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjasdson.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nknwfanl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vnlaiufl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2voeefizh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2usdxhbut.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kvmcfrpf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ajpkmngh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uqiznsos.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2esexhmso.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjqcwlru.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wilaldyy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ssnivnbn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtcvgsxz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gibkzpoi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kxocnqfb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2odwpcyhf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lgyuoxlh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dewkaprg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sxdgiabt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cbaczzvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nbwgqaac.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sbyeeyev.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qvpwsnsh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nusiydkv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qbyybvec.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aqukfoxz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acykgfan.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wmixawih.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fdtmzikv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jojbdwfp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hqtimkmv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkdqjyze.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nesyrldj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sgssfson.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sznmnafc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuwhvvot.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mjrofidh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2motossov.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2enwhqzpt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zaggkkac.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ovjubokz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xilpdomx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fywtptbt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mzlebczu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kqpifupb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zruzmzjb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vjcdyrdz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zckhfpyv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2srmjxfkq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rmjpspnb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ivrogyxt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aagvvcml.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vbqqoqbi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bjvswufm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qenngtmb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2xhjfyjcm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tbmrickr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ajobuqzy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2otgrglgg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gqpuvnyh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkiuaoav.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2albhhglq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bezxexwe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2edltdclt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ifkurhca.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nrhnpujc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yqijulub.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ppaedlcr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wvrpogzr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2aoegrnlj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2aryaiecn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2loqyfmij.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtnpancs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2puygmnml.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kcnrjpli.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tcljkwly.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2orcekxlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anfevjoa.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jdwdcnzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlmvmnyz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xkmnjpce.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ymwisikj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snkmwgrs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yararikp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vhukhchv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwsqmpxs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tgfogoac.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2syogugrx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mufisfgo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dqvvpctn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dfpusxri.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiyjascy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sdbogmqo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rgzuxyrj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqsovtpu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2skitvupd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yujwmvbw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccmckczs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2unkylvcv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zjlsnkat.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gtwzzurs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dnzsyjua.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bupciesv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2scffmutp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rafksgvh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mszbzqlj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2edweaspn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2tunpkxqa.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nxqgqghy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hsnmdzie.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jhzwqruj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bhabjjsu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcbazlno.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2octujcgu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mgubvlgl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2oxmnjmfg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2eymqanbf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2mygwmeye.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2sssnyrsj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2clghqvad.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjcjwuvk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jepdcher.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2rakislwr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2iuqfwtcd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxrkmiwu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pieltxfn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lrurxypd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wrlwpmph.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lmpbmeez.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cwbwburj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cayyofnd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2vydnwbpu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2phjtaugv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ddildhuj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mbhgjqsf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ovdmcdtx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dsncbgjq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lyokwdlf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cxgronzi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wtuahenx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2icblzbrb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ytawgckn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wgjzjelx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2yjmoengx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2eyksoean.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ycuxygwr.html


<!-- 参考信息 -->