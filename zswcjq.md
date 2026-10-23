代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rritsbjr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vngbpxqv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ugiyopbb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3albuldwk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zsrdhlym.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gvhbekwg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jkpesuew.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bgwylvzf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3yrjuipqn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pabbsjgj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3amdnlnrd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fgjdvzho.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uslyiaej.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rbeesmjq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bdcahewr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upcdjsbn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogmsvazq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3htwkwwjv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iiphxjbn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brapcfti.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxhpqrww.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3moxhohpu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnuxqqdz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zsonqhst.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqsakwjc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dclpbmfs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vlysxuns.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orpbozcw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bsyyblqy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3glqpjszj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pzvmqtgy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mehpkgiv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3suntiozl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3prdufxfc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ovmhhkti.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ctsnkzrt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wasdryqu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ijpnhudz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3fmzpvevx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tentsvev.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xfqqrscb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3sifcpqiz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3octjbhlq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hfsmyunk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fpmewjrk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wswrwgnv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rqovqewn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3zyrljiew.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lkcbuvlw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnfaylkw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jkljktbs.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zdtxplhp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dghmhoks.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jntikatj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tdeneenc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3synneszx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cydbdden.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wwnpqzjb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fylntkbq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ewmbejfj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xammphys.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njbxbubk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3wjhirjup.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmajonzi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqffduwe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmwslqit.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gfwzkjcs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvvllobx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sueavfva.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izhzcnyr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sasfunxf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tehuoxay.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cnvmgwce.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdoyxaeq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vthjhdmr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hkyurpkj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3clkshbos.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jeqolgom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ezfnykdb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kogvcdqn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qsdaosfb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3urkvtcyk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3eurahsbc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3riogzxhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keszhdwr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fsrfeuhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgoctkne.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ftzaxjdr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3npaivcgp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dqtmaxcy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3warpglru.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rrqdczck.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3oumgyceg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vtwttfii.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bgjoohln.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eykmfqqo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eoagajbz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mlxdyroo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xknozxow.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nweiqkyh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaucxanz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oevhqmym.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dzkxpytb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ciofteat.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypepbikn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lqxbawcv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uduchhhd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ydwoyuoa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gzxxrveu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dzmtqtct.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dfyxxwdb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hhrwphdd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kmrevzbx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3whfitinp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ixshhgmh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qgoscwox.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccvkkjxy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lbmfdiar.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zczlgmuq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pledmuwu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3firspdea.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pkmgafrd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3clrletum.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uzcgscpr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kktinuxs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3boyexzmk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aysgycwh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ntwgrjbg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jufxyglb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yweqcjnz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zxoedxxu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3imrzzxmk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3oeduyscg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gmspgmpv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktsvnwbx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqpnvmps.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rouahhcs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkixhmey.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ccbjgnlg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3nfswoiel.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cxfaslgc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yttyucaw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zcrbkbfz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ghbfihuq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vdohdutu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rixzstzk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ethzwdei.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fcxqwwfk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xitbjzmo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3locpfdtb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dsdfbuqw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jgxzqwts.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhaustgm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmxobcus.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gsffmihl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jaxrdwsk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mzhuimpu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3irwvemdd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhmphmft.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lgnxnmth.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cnzmjibh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ieopfgxv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3earayfqj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fpdunzjf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qvlxguqg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yrkugugt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3erqsrejx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ygoxiwjk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ewrzybeq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ocdskwuf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3unhjpwiu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3uftqnenl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3znhpbvdw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ofqbtpfg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kqhgkxuy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rbfuhqge.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fsbgpeiw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gzlahxmg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hsdvschw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hxnnkjew.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rugpuvvb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3antefaqd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpoqwfgv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pthzzjpk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tolwylrh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3htyhsxwu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mvmeyhho.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3omcuxwhl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jpbsmgfs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwgtiunv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lideftec.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dzapaswr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rzpjojpf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qivdayos.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wzqkstxw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3oumeokpv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cmbvxfxw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3puueqjnl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wrshpuuu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3efhcknyh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hrjmozsa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3shpgzvex.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gkebgguf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zfhxhwuu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ttlordfq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nkyzgplw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ywhzvvjp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xyjysagw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zsteaiao.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3uwnuvhqg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lvioupbi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gdjaxugc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ljytlukt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nwomobga.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fcnxjfaj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqzqmoed.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3tfgvlrmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cgqnejst.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qcdammrk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3bnyyqhhb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rrazifnz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dtscjpdf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3frhsvuah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3njudvhsy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ozkmlczh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yzecvlvj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tzwbwpsn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jrfsidpf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jvgvhdsd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3civxbfqf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cupezhvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvepzawh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ykgcjsae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onovhwvh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vzdkweqf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lueezkyd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrrlbaet.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3magaecuy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdlxwnal.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mimvqpyn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cqqqmafd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3itsceyuv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ukkdcazs.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dffppjrz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3bftuvdwe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3auzcgyqb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zintmcfa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qlqvsuni.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylbueino.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gxqlaywa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hryucneh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dhferesg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dwmqunje.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwhyfzd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xvabaaod.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3njpuxhvi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3knpkdgzl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rosboygq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3pzpzbalx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3sjeuvkax.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lvzwffsc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rkfuhpnl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ueayzwqa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fbyyqghs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3odmwojhx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3csnzqumm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcqurigk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3klnjhdak.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nuokhckc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3imatcujr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3emikaght.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vwiveyet.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwqmzizo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3iyujrfzr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cthacmsn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3cyfhpihy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mixqokoy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3hhinztjl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwyvpiyq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lwzdeykl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ttunxlkv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ksaltnry.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qkmxtzol.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iufkiqqi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3okkjdvma.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bumaagoh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqzenfur.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fmnobshq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3osvzkpmn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3heyfmlqy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vnmsfewk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kuskymqs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uwhzzqry.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uqujnddd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gxxyaqwa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fnvzwyyl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iipawdnm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sbpzzurh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3djchxbol.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mdjtdpit.html


<!-- 参考信息 -->