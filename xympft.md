代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hszsdgzf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hkqdbntu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hfribmfg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yeysdqly.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3glpapogq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mupwaiyr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fqwensxo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jtgvzyww.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jkhxvbqf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kbkgnoyq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ienveoeh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3envpalyd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtyoqvtz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bqaydsph.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uwoxhsna.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcmmdmwn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ueaadowa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjwjzpaq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipiqwdjh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hlljetof.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjdtorkj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcitvykm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mlgzpmix.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scngidpf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgaqbkgf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zzmwnyuz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3clghftgd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gnbilesu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uatjhrhc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3muetdwid.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3szhhwuas.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3smzwhpcm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vlujdmmg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ltakxkpt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3huksajgv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nmbxacqg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3iwrfhdcp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqvxhfrm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hvrfypnp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ltefstgg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bnrgooob.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qrwdwduf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ykcurbtp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tfcroxhk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lvuwzbui.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3erosxnof.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfgysvfy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oclftire.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hjxlltmi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oclodvyk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vtkghlnz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvqmeipi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gjbrzzcl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3onwaxcrg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3inablzid.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fasipvzg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntxfplyt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaxxitqn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aozylmic.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yuvlvhuz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfetecut.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnsaydda.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tsajhhpr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbhthacc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lcntkaol.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxieeeeo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbhronlu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yugwbior.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tmlbghbt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcoibwbf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yxixexrs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ivktutjo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3umjgflzr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xpgeljvx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wnvodsci.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3huuhbtvf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qwvfhfwh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pcbcempo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lbheumrp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dzegggbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apbsjglh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mxofkwhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jybomhvl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3oysnhrpv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ireaasek.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqjpkubv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3moepejio.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkynbtog.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pzbnvmbl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3grzqlhmq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3clsfmlvd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ureslysy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzpqshfr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qvvssrnq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tqebmuoj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsnnbmdf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsicysyn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gionacdl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3flheejat.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bfqqtnwv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyenfjdc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nitezkwm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wkklmhlj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qnljxcvw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mijgrcph.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dwpykkno.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3jqyhnyur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mnsvoglj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nxfqwlxm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hxonlbyg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bcpwpjvw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qouidmun.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijolscte.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3demlypef.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3twfaxriq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlftshfq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nsgbjsjh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gasnilyx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3suhiaopg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3awibrjmr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3idhoddeq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pcbzmzmd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vvowofdh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3weogkgbl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vwcddctd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dvzjsjlr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjvyrkai.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vqpkcash.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3umkhpwlv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3chzxnryu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hhqkuujw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evdqaogb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wrlvpefk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxruvyhj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vcijoidt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kiuxnoal.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wfwgsozs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hetzbafz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jtybkvao.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uwnippnx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cjncjodl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ibqqfmhe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gihohtcg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vjnaoldf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qxgmxiud.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xvwahgeh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ytboupru.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vwjxbpop.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3myztjtzy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rxihyuhc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kbvvwifd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dpxpgrgw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mwiqufyb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vksvustk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3edlrdlkg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tcyfcgrq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kebggdea.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3svfpxwzp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3omsslzro.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fbfakvms.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3iylzrwyd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jxibaqzg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3igqxriac.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yktbrocx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vdtwskfd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fhyyvxef.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nwfiwfoe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zgknfkzr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bdfqwbzx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3owvndepw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3oysmbsxi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bvbpqrzb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vessmngh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ghbaolwg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zmcvfnpd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ohpsievo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hlhxcbaz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nnfrkfeg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afnhvaoa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wbggqgnx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iluqcekx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3lhgnwenc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gddhsqxa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jahhuhxy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyypsjft.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gylkusud.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jvpzjrml.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hohtrsbv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ufufrjaf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sfkjwwbt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lrddikop.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yhqicrja.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3udwqdzsz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aiosyvav.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eygofvwa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cezxzrts.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3whkpxsuv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zzshqkhw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bfblwzyz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3oggrckho.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vuylhglt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oifydcdg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3oremwcfc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tylkbwor.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jxnugbpw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srnwuwpm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3alndkawj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kcprknol.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bopkyuir.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xxxkzrhy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qgjscnyt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mwmqxxcq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qheuyhag.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3snlpwfll.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dprragnr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqsyrzy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zsktuopi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nnqxepma.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3lisixiku.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lxolcbfg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3upeekcay.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3janezdmi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgmhbasd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vtumvdxq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ejektlcp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pcttpcwi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qpuyeyyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxwhugyj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3onrnolxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnvdzxwx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bdfixfwi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3rkaxjutt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yyhvhhus.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tljeackp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kpzfmbzc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlxxbqzn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3swxoiaef.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ictcfwgm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixolrtnd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gxkjjmqv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3jnyqvubv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aixwtphu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rtdccmxx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imgbnvvg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ezrlfxir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ahmnvzjc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fobwraya.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewntnrem.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3coabxgne.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hfufjthm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kyxllsyd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cidmckxp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3npccjjiu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xfmplkiz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dtadcdex.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3nudatxde.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vwnkygoe.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3yxosmjhr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3agskwyda.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tayqmzki.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrhynzud.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3smmfdidh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyytjzqw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3aanhnsge.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nzprzvac.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbxkxbpl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kiqpoejw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3obkjgyjc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3edkrahmi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3oqxziolp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dwjehgsc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3euisbyrl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ycioqufz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wqbeyfvq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmpbpugl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wzjthybn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3aghfjcsf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ysdmqygs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bjllrcie.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rfjbdimr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3czotnxsv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rsrmwkox.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3osrzfwhk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3iockdnzd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jsaldife.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3lbniwdwa.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gkdytjlp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3voksiiqo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bwyeqzrm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hwntmyav.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3rvksrswt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3sjamshqe.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cikkfqjt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ypnuvghj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3uuozxjlx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ikkmmxes.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3exkgknyi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ysaommoi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3pilhjupt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tdteoaoj.html


<!-- 参考信息 -->