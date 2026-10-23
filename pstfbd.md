代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nmoytjdf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3coeogtsy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dinqrisc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3btyprtrn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tpqeolqo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lhdkohsr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sqjbvobv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mydzeaou.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3agbrtnho.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jvvhigwn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3udocrkmd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mokvicdi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gvoznjdk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mzhqgdxw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jpkookkb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czmepktg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywescrwj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vbodfisq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3jvqndbeu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnbohmxb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyqrnnkr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pdfuiped.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imszovir.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cwkqqczo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubxfhxkr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtznpjap.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3axsrooll.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jlbovuld.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezqasyat.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vkxgroka.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zveyxkxh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vtiqklmw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bfganlmx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bfldkblr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dkuyivyv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3cosbgcrw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xjvaalmu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kaoljdnu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3frrvbweg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pvownqrg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kmesxgor.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xdnfrpgg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mfyvqbrl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pseezcdy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aumrkyve.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wunjadez.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ppliszzl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ecatshib.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3iyvdcngr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umjjgulb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3papxyuam.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eeehujtu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ifbsrubb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hflparpt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jrlojptx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snlcpwzm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gxvymhtw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qlmsaycw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gusvohzo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dqztbjow.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcslkeuv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmfqngqv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3somnvoly.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppgoftwn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tngwjyig.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oknttexc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3oaikyyir.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipyunwqh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zkkmbnbc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cputrfou.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blqqnjbv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iygtuvik.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gpnmouvh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsizjwfi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3otpiawei.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jleobtbt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tenaqzhs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mrsjvrvy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gsyxrrgi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3poqgltrm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rtrwnpkh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zhkuucsv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zroexyqu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hlahwcki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mcvvwrsl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ojkviykg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifdrqbvd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jbjemkpm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vhncbjyr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilwbzywf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3huhkubkc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkxzcatj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iffrzcxt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dwbghczw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dksfikif.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bmlrrunj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzayptps.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qcqibfna.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeeutaxc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zckjpqie.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3dapsymbt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3offnfrps.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ribarmjl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jzhditqz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pziskajr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zoqdozbn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jcdezbdj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3basojeaj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xahxvfvf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tsvyhaqv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ukebadnw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zmpoeljh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jigiaghl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3iauwqyip.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lupwwgrb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jmmlbcfm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bozbgmcz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybwydvxo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqdmenin.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3umxfvprp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xuxnibhq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3idwuddll.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vpzeozfh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wftroaxx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fhgijmuh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hjrobzrt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3leqxayel.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyubopvq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcjgiihl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cyoqmyhg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lkkwikwz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3spvetifc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3yiomsnao.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kyjcqkxx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcrrqtow.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mkszqknx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgqjhyjo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uzoxdtvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cujrstmk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3schllqli.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cdrddkha.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cofmqhkv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lagrnnip.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tpkmppww.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lstyuhze.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xpxjdocd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pnmxfgsk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qhmpqclk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pbqtbrko.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3amdkbpac.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3exbhykeg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vrtpcnjo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3apnqsxig.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzfrzvtn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yifcudzt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dlheukuh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cjkbudqu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ysoasalz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsmuarhm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qdwygeag.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fwfdohxv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kekbwfcp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uzifmewd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sljxuors.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3earktcdk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rjlbprke.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ieecsvge.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gmberdrx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zqvfvkmo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hefvezfw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xmdrccxq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cmvbgmgh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dgwdecrd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3modxwtxu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3sdrpyasv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cximhupw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3luzkxrjy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wbsatvvi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pbecftbb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wmuyiylg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjdkxvfz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uubqczju.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3arlnxfbz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wkklocvf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3sqsyopxe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3invbuldb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xcxenfho.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3achyufqv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ryxbzmaf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yklejusg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpclccc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mixthgwq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3safmgfay.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kvwdaljo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uveioonf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3oektuinh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3snuapazs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aqkszrxh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vijgbkls.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kqanbdga.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hopjkdws.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3iamjtqem.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rdebkiqe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gdewlhtg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3aaurlgpq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qycnashj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pnrgnrsn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pueqdedn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3whrtfkwe.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qiodtfin.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ryqkcssu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3msfniczd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jbqmbnef.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3damqqhka.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkfzaudv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wzmgkwsr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wtpdchrd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mfmsialb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hykkzxjq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3exymmckw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zsvljzyv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mjpraijs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rszgfiiq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bnzbocfh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3xixyrpkl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tuzmijav.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tdlvuuzi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wtfmimmc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lsabcten.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dqkrnild.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dtdpplni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucrbwaid.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mhykrkxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jldemepp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vcquljyg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3odijrtrg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jwazlsai.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iiihrqho.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrhgslmw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jttbhhod.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fjweuhhe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3fzcaplpy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3llmqubyr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3hajttmya.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3serrcovl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aysxvvvd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3joopnmqe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ufbkshth.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wtrsycav.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3eoekdrmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvglcmzj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsuxqylj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3othtmntq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dkrvfnzn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mrammugj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wyrmtvml.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3maeqewto.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sceleobh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3stnicsio.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3iswpbejn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3btblydfv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3alobuplv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qxzjhnak.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xkwlsyln.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zbnsvsvp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3akgbfetr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gudzeyrf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3gfnklsuw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3eemixjzr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3shpxfpwj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3aqathitb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3pvmjvtjg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pweofvpu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvbaamsx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjtcthey.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3mqcwrurs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ijuwezni.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qplvmztz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmqpzorr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ehyxxska.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jlgctttc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zjbgmoss.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qqodhlgv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cquwcumk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rlxehxxf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fgslgyzn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3buxnswkq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fdidjgkq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3vwsdcypx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vzehuids.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zhzfpowd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pmxagtck.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cpxgotvm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3fkoxcqoh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fnqunrtp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3tvyrmfec.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3keyxlnit.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3zzlggpvz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rvzksglv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3hiecaote.html


<!-- 参考信息 -->