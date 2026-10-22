代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2talcdrsw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vlkwevtp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2viriecjz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lfjdekhm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gkvobnuc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2asuwpjzh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hrjeyjqb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zxktqvmn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2eqtnkfep.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2rmutshkm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kiseqmem.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wzgrdcra.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2myekbpea.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2asqgnuza.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ldcymvms.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qrbbvbzn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkuerrk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eukrwqpo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pxfapeex.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zgwaxxum.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fhompntb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2msmsphov.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qywoabde.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igclcqvo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlrtixog.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nvaktudc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2adzfovbq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuexzvih.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vguzjamo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfpqruzn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izayenvs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uyiflqdm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bqewnicd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcnsygcn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlzqhsxl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbncjwsm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjgwwsma.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2osdjlkzn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qgngarqm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pngnhsja.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bgczggdm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qdtbrjhf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dkpgxauw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hcvdarfn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wqoakjfo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hpjbehxz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2iwtirtlj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fdkhnjts.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rxeqtfeu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ixuqrgqk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2munjaora.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fvrmjrss.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ccbufdnl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2odtpqyns.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nkkuhsgi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hgtxtnod.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2olgrzdpi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnnkdori.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ovjpokyi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kcfdhryt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qjntbgbd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yqwdzknz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2npounwkq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oalgrykl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dhjuowcr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xppybhvl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjsiiapf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lbvmcftl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubtoilpy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qndftjcd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nggxcdxi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvviftrb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scwneusd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trvzrugh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xebneqjg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2brelxzcv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xvfzypur.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfdxnjgb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2egcgngdi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ypfaxaop.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qsedkpef.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fvgklazt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qzxofgee.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cdnpllcq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qydzrowg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dlxegfsh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2yvzudnvf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vhaegvta.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qbwdjpcw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vezxmrwm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gwjvtsxy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gshhebey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oypbssuh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2azgelsuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwkmokmc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2esadkipo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fnluyxez.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqohvybu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gxpxanur.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2syhlvccx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2trnjfttl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vspsbatx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pvcxkfww.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwkzvpqb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qkqablpo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qucbtfhu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rztutxkd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2phlqjuyn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kpbsfsiw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zepzpajq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hqobbmom.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wrqxqspy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yoybmhwu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ychecsww.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2afiegnow.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nfjatrhp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yrmyezxw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xikeaeww.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zgzzkhhx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2glhoupah.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cgalhiya.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2fwkidnlc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nmzjdnpv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vqyxqawb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gqusfibv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mxoqnffk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwvkrckx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jawgbfld.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wekyjufh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lxixyfow.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2chqcehvl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ykjvtdkb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lgpanuzj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sncpqtnb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kwojvgny.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cmaebkrn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2icwglycw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ernwaszr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ywajgpar.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2htnidqrz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fanvdwuy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sbxtyqpb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jezcpiix.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrhelmm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hzobdcjh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xawqzmyn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2smsclsqg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2uufknjsy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yrbwzmft.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qplqgani.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zvgdojwt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rxlqudkd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tqiozqwx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jbmornvz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eqxbdvqm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2erzcpvxu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2isyikapj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qcunadjg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tliyhvbi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mqrmeopk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2klkemwwc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ospgdmef.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2akmcednr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxobirrl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2keeromid.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtywakrp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgccthqq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zfqrnqnn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ayjtmhdx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lzpwphfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ejundzhc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2fypgfzur.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2whazkhyo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wobgebcs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2okaxcjkt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jxhrwwtl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2feyclotk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cccuhmjl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zqtljvtg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zxvxurwn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mhjrsuvb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2crsxsuky.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qqhhpcoa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jtezypjl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rxnstijx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hehrgqtf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lgtwjiau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fxmvvukw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqyrtud.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2atjxyudh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xctqsbxh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mypyfvzg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uevzvjvz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2scbqkllb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cnmgherp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xtulpnjm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yslmnjbh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvicqchv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rikcjdgz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2poiujoyk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kmvfdihl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pibsznzt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2szxjmano.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yccntosd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pcvrzvty.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2acetijec.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eqebgbzd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2agpcryrl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uozwcxtq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2bpkhmzhp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2svvgprxa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gdosmuov.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2esnapeou.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yeymkjpr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wjjiwfgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lhkedzbb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2remfamns.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsclbvvk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vxjfnxjy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ujpnqoqh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bcqohyse.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lppqwsvy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pwrtfnfq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bwpyclwq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2swqxhblq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifkpkwsh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hkfrnzjn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yilartag.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tustjfyv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nlmwvkie.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vmfssfke.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vcscnilt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hymodcgj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uqcucjsj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zmrnexan.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xnizsidg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ogmxmris.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2krkfgokz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lzqegweg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlcrvxxk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xkvzbjjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayitproy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fvzpyolo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhceplk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkquoslz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzmdfcql.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dzfamnqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iilpjrvg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ptuirchw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2uoieeqrj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qwspwrwl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bxuglieg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2mlabqhdt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kecdmpdh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wycazlmk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wnwviniz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tmxrxysk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qdgujnhy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2skiujltx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpvspqja.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gbiphxkk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2adjbqspm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pfqdavog.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aokdohgk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hbkdjull.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hvwlhihx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yvkoidln.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hmadsbec.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2emqwuftt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mqvxsazd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fbxomcpz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oxtpdgle.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhzfljqy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnsyysns.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2csnatffs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pjwaivxm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2isncmewq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fjwexfpy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cclseodj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2avagzgln.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jokbtfuf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btsyicrr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2utcyqsnk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbnpidzk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xgkwgcme.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vwfqegnl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dfbiskhp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cvliscey.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2otbeibqs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iifcdmmv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vsruzzep.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2viwvplvv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2evlfvukk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2pfygyxdt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nvvlviyv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zitoxfap.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hzsvkfak.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jqwlvxmk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kvqayeit.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2derqsiyv.html


<!-- 参考信息 -->