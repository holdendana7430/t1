代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fhlxwyiw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2awiqhmhj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2awdkhryt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jpvqdwwd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kteqoxtb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cpztimqk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vieucxrs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gafthttq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jilqzhdt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wgtitcxy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2znpseiyt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wswfvapx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vqsxxfks.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ailgfszf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bfniqihr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jxtfxfnu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2aloafdut.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pqbtpxaz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dhfeqshu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fabvqhuy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mndyeasl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2spnkwxnv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qkkuivdt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuvdnbam.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izrvmncx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2puoeammj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bajgbqhk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbpsfymm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwprbtgf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxbgpceu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpjtlxqp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzthylii.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xutaiyum.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbdcodcp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ouennnpo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlngvtjc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eubzyerr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dfihudkl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cauuakhb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tupczmdq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2urtaywlp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jzwdclhg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gglpospg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2azshsgxj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgagkcp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xvwammpt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fquntcwr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2eyhmjdbz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xjlrsacl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2afsdvnoo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2onsfyvgw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nocgusij.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jaocsklv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gyqfjzsv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hwfrwsib.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2mwmykjcg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lknytzgw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2loytxkcj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hoxyjsbh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fqmngdws.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zqylbnwq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pphxlwlx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ymoshmur.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2skccfaop.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vkjqfdfz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2drcnscki.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbtxpdlc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2swdofnxj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irqibqoo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pchpneez.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ayebxlet.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilihpykk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uezijxxn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpbuvnrt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xtlmstol.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqxewnnz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hypiuqro.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rykyurye.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mruquduh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gtishurb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ydyrxskc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdzvydym.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xznqbhfq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2umabyiot.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2imiohgdd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ipajvuxc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2otjhwolh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yunzkdjy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nnosiccy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2olamibuk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tgcdjwgs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zibqtlkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xonvsaft.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pusfeqnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffcmpthk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gvdkzfzp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dykxtayp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qbxchgld.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ukpevklm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qeptcljp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsfybikh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ljpsjoqv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ycoecnlj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bxgfvnib.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xdibvida.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zmfzoxel.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ffsltore.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbjwfuyq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mghbhgof.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jngtvhex.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2psnnagbg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwemwrkm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gjwclyzn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ibliwcsa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ebewjwgk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dwjulrvd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pvwnqvuo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hphqlied.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jlfmsqkt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2emgyayze.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ycqxkaav.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sfedthgh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xpjepkgx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2msirgpqf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uucoowwm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgoqrra.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eetydqob.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huewlofr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rcnmfgxl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dwkbhmmy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tzvvvmfc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uvyppmxh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ulyryryg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pwvittzd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fzsxrasj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ceppxnwu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mqrwptsb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fwtiooqz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2psexpexc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dqmkebge.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bnteovuc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2upidkgir.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2isdwhhbr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjbmnrgo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaegwaxr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xtfeqoyb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kgjeogbp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yrcenrgs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qwzeuohg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2odvqdadb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ntcwafko.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ypalbjzr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ddkwlcgt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bfmtmxxf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2erqcwgdf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2eocegvvb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2msyhiauq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pnarjbeo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tngomyem.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bncapppu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjcssjzz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2atvdogoh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hfvjdooo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufzthmif.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qjgviyxo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2evrzayga.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptykoiha.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ovizbnhd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bfahezmw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2igmmymsk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xpghkqnx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxrjtxrz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uvoxompb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwhjywc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwuthwbn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjdcoyph.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jylntfyh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2eromhjcs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nshkqriq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zeueylxv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lybqxqpg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wciiummj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xvkgrvoa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ieihwume.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ranvhslm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2upzwnfcd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qwayzeyp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwzxnybr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbscvzfe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sznrcumi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ptnxwtqw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2urkpjfiv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2clqcmmvo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bebsltcu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ovlrhtrp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xtncyklv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krjlvvbf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asuicykl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeddlgpv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdwoucj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tiwuhhyz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tkeycvqy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qkowjymj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmgbgxbq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dgykgvyo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2inckfgjj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vjrbrwxo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aeqwrtxa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ukvwvphr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ffsygxaz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ynokeypt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2iumwkyxv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ycektgzy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cdohehcr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qbezlxms.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vwbtomob.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2txrkncrj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzlviumc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2osgndacx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ljwojlmo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2aijrowal.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bawcxevn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wzlcxior.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2enwyrexl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mvnmxdiv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2efximypn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tdzmrexb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vndjynie.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nnsebfqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rnpoqkvp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vryqinom.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wsqzupcc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kdtteysx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rskawsim.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvcufgxc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xvkqjiyw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gphpkekc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hoyqyaye.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ysndchww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2molupdmt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hmkrptuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdmuaxdc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dbzguwpp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2utfbmrdw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gdzzkzux.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2krzsmxkw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vjdkmile.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpflbxli.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2olqflwgv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2uolunwbu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2macnftvt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2jnauilby.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2vhreloke.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2auyxqkdl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyzcbmcz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2venjhkei.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wtxadrrt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2iztralvd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ewfsbsyu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sftytnqs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2evlqueev.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bbljlama.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pdjcjcao.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tqtmtklx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nalyrelc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ivexrjws.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2llurwiji.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qprqavik.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vmzxkrbi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zommtgkc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qgxctgot.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2umqxrmra.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzkpzzre.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bictasml.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsbkmhrp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mzyetrwk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ygviijmm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wndopnzr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2btashgjo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vdmlgpoo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kbqjpnzu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htlttbus.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lkkctdqc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktczfcez.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2atoyhvqm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rkcpfnnc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxruoteu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jnhrlusj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2afhexain.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ozfcebsg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2aarcqkgz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2atzquqxh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nlcfokya.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ysovjati.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2lvcmpisz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vjvesyzx.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mmkxzzbs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2lcmnsldp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oyvczcmt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2frvcxvui.html


<!-- 参考信息 -->