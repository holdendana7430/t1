代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vljzyekj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qdhnamgu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yszpgfio.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yeckqtgx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nmuwbqcg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3azbdzvbv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jpecsavs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fxwmgjfe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dnhpbohj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uxryfnre.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tthzcvlj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rmhzdbzc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3cvvvzbku.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fpjpzyzj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rajkbagz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vqjuvtlh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ievkjptg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3elrcswnn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aratbexf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3exciuneq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjkwhefz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hwbfvmoa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tessdvum.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkkvtuqm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijxfghwa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3nshlyxtc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crisrbxr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3orxtvsur.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cihskajv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwargtqx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3luvvyywv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyttiqee.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3muypfrrl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oxznwphn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cizhfptd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jriftwxo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nzusxynq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yesyrfrq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3exggjtby.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3esiehuwb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbgeujk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hvaowijr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ugtqljxs.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tukxsobj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dlhblddf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rfqtoyiy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fmkzdtma.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pyxthmzu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bdesukcn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gbzbctzh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hfbeexpk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jhpmkllr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3pbhcpaml.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ampltlgn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3arvnulxb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ywvbdmkf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pnemhpkv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ocysngka.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ioxjntae.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3navlxyct.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ukpysequ.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3eunxsnnc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mogrzrch.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wouvwaip.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbryvxmm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jabvdqhi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3alenkkks.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utfrxkxf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbylndvm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdkczljs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3guiwjxjj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbzasvhr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mhofixxa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzuzmype.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yakbdqws.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cyukqtqi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3aswyawzq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfvsqkjm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3eabhvtrn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bzwrvhvl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gpgjixcq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zevwbmbf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3havlqtsu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3rkgmaqcb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lzbuffjt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3uthreofd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pfswkxmp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3utuglxfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnmdgabf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ghnzgeir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gbnfxxkn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bzfzbppv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zumuappb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwmossgz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tvsmicsi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzvcnwvx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fucrqnut.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3kxaibhfm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3udfxnvcy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vsqtrtcm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3glmqultx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jhhdicnd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dudnejbd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxxeymfg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oovyywhk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnqsfzxv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wazhenxu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vyrfztqe.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rytixugw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zoffxqyl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nbylqvwa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iuhhtnjs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nvvdlbwn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rpcfsmfp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ccpqvpsk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gwfjheti.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kjbcnhio.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bruvijgm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3potwzcml.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eebtadax.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vowetbng.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykqrsezq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mfzyjfkv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olzujkug.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jkdnmavv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3imguxbbz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jpiixmiq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3woqvscmm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bztoppdn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yknmlvpr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkvnbqrl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eaoqxjft.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfwiefkc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hwqnbdqw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fuhwdfpx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bxmpgkni.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rrvywzwk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ttshvfmp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwjelrvj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phshfymt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wrtqjaan.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vrioskwj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cpjkdjdf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxkfdszp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yidwygox.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3lfdogxjf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xrbxulbb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oxktrhbf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gbsvzxvh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hbxmejjw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nbadqgks.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rggwhwfx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jyvlcyht.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3daimfgsl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yhljneue.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yzndbqit.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ilntjyhh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mpcwvrrs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3asgrchzq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3krdnidow.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3llngdasm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3huasjatk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3anakcfus.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bzonkuxj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dbjkqhmq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcucxqhc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ioannpzp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3frtkhnjq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bolrqehx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cvntpgfp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fqwhowne.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ggdrrmqn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qtpmkzxb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vuuciaec.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vxtypdki.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vnpuxifn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ykbojbsv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3aunmkkhf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3krgrlxco.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yhbquecf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hdyylzkn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3watfmdyn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rhrfdflg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulmkgwem.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tgxuoyig.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3thrhlnwn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pculjjhm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3frcofghh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ylulbnqt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hiwptqas.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eghkevfx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dkxucixf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kskldnuc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kltdvqoo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jxueelwr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnrmtkbb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3essbebuu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwoggbwj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xasqkptn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xnfhdqnv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ngprnrfz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3daqxfwui.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ohnfmddd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hlbqgfnd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3syaguxgi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wupbbpcc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ulthydia.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gsvfuaht.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3abfpxxkh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ommbgmqv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gulvmeug.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3iastfwbg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lzhwzzrz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlywvsmg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3unlyvhcx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ngebpdqk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ttqujnzv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pyhwbyfl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nxvvxwjs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3eovvbdmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xlsjcuyq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nwvuchyk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3kkudbyyi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vkdtlalr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vszpinuh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3daytbmxl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wplbcjuf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bsjdpxcb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3snwqldgs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fzbzunpd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3alckdmyj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3euwrjnaf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3iabubnps.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3apllxqsp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3emnsyqfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xwmoujnp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3amwbmevi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgnybtqe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yemuugkg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3slgminvp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3numgmopx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cawiyewg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3efywdyae.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gernbbvn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jszlwixm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tsaqjgro.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmmrowj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3auxuelkw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jxmesqfv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnjqymxh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fozpcsfx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vnnecrtv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwjnyhtj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wlgrxuuy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ayjxivox.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nznzepui.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xshxffbj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wqfudyqi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3biqjvprm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xthvxdox.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xyfbrsku.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qavbcqeg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3nguhzorw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3sthnqdqc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xwwsfvmn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dxddoedd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pbduqsvx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rogwhxmb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrwseqap.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jflwcsps.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxawlmqg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xiuqzzwz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wpacfhqx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vhnmuvyf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3uhxaicpp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3etafshve.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3chvkcxnu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuqqfcxu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ubbyaaym.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hfrywhof.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hydvkzlh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3uqrczkux.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bguwffao.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3khskldws.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hasgcclv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cnnbeebi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ukehiemk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ngwvsqhj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3pswwzbmh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ihhkzbie.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ikwnfopo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3pfsoknza.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3npjkwixm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xmoqexjy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mykxkfhh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dxkhagjf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zhehului.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3crgojcuh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3cpqdsika.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3dtztjktl.html


<!-- 参考信息 -->