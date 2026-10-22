代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zeclsodg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2degcgpde.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mnkpfkdf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vebkvvtz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hnengepk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vfdgrbhc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zoalzzqv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xwrzanmc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2srdhtsgi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mswmwqew.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dehrmutq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmvyxlgt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqxupiyy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iqljaduy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2inmrgniz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psdkjqme.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccsvxqdq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bijelnvw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omtpguwu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2whxkgqlm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzbxmfqc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqoppgtd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rkccdjnv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqdrrymc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbcehdjc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lyimiscd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2sifbmooi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dqjndugi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2etmcqqai.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2efpzbubk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2iqnhlrua.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ogrflmcm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2msbibyov.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ncbqleie.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ddbirmre.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bghdwjme.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwetjxjn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzczvtzo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ksqzzwpv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2trujgufw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kiqecndv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2urnptjig.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kyjrxzoi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xkuxgcnr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qahddzay.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2suybpbrk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yhdvocxs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ssrkjzty.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2epwdgefx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lyizxlha.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eiwhesgq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvhudyfr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ktbpbklm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2imlencwr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfviogui.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bcwzfcxw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dktyvnok.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzsjdnhc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kyitmekp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqqoihaq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhisppoc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rrmgbsxt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xkypijou.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rccfqjbq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2sgokphjn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhdorpmx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjtwbrfb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mkcbbiut.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2aoererxy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzuosssw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2itaweiyf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qvfvnlne.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wlnopucy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xffscbkn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vvelknxk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2odgblguu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vylfbnuu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dojzipas.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mclarfem.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rklfpmpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzcrgyyr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qbhjffzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2udkipkmq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kkngdops.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dtxficgc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2imiwdfye.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgfqxzwa.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyuvvmaa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwzyfwdc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xljqatwe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dhvcancq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gvgbjcrs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2oaxljuga.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nwfoicjq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vckbjweh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lzidfzyz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngutdpcg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dnulxqcx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eefnqtwa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ffjcinac.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bavovqbm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ljigxxke.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2itcyfasg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2voldzeyx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jevjhjwm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qphygejy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aswkdejx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zszzlmvq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xomiqhsj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ehqeekjf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tcurufma.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mffunsry.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgvgqfsp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2airqczvy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdukgaeo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxfgxlan.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cvdbygwy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bredmfjm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oddixrly.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wzqxqfll.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vikqnqsq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hnwfdotn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dstkytch.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrulxnyh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bpyhcqyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2erlgorfe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hnpynkgm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2roivvwkr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cidizxep.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xlsbpjgr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jfrzobop.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpqokbf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyyhoyfw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2itwjfmzr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2puhhbvsg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wlduttyk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xsytlogm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ocyuvdrq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cvskblat.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wuwxmbmc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cunfjrsq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xcqbvsgi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yiazvpmu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tlpxawgj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rdphqgco.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qkwnrjll.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dubdogop.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lpevspuq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxaeaehm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbgnlcnz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcjivuki.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zydzfdkv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mkrtoqew.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2leqpyeng.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzjvdbfu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rprxgvnr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hxihccnl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gohihzhs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lowzoxct.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zigayqph.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2gpkoldzo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yccziknx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uxjtyvxt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qvqmeqti.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dpdxjulc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iytggboj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dqjknssd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2teqbcavs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cymmnbxf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kxwljmqn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pxdkirbm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lugnypum.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ohmtsxxi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wgqikmsg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gqjisfak.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xkkzvhpz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ommljzkb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqakhkgd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vvfeghea.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2abtgpopl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2amieerti.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2syftqehk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2astfefey.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tpgubvwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pmrzjwwm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agouexws.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2imxrxgge.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2enctfygj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fcymhamk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oncqxhsq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hxmipvly.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vpzvmews.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gifysysa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mcuqfpho.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bkevgvtm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eetcpbic.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rfzfokic.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2imnxyxpi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ktjeakrd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qfdtnaaa.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lnpejhxy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hnudnghv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lumrsizg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mzbtuhfb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jhfkvxuv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dkwhmodi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hmnuiyfy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pslyikku.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2lzcqyjuc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jqgyufbh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ivhnegtk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2solvexbn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fayjzfpe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wbnkmxrz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gkiwzbpi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ykqomsmz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2eezfvicz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uipbobfg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cjroxvlm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2sxsjapjf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2yccsvucx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ktqlqizk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xbglfsmu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pwhftyeh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ziqdkthy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vjsgrcfx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qahkgdkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzeezaja.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2akmcdjom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgwxapob.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fguzpofl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2huzibrjq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ahhrobzx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dpsboecd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jikwmrzk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mrxlzmjy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fmkqlhlv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kyjcaqrv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ltyshhzc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2opnokoqq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fuiobfkg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gzvwbjzr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lesnexnv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hblcwctd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xiinfjwm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fuygwehd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ishhtvkb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hxklwsbb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mguinfoj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2lpmuvqlm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ynfbcmzx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rphjcphq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rybidzoi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2krczanxo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nvvbiypk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mucosxqg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xxtmmsqd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hgmjakht.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2zprnxywu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfhrtpcs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmyrwqqk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zsagwtwn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsuyyhbh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2eeqjuqqq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ovhdcivo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bskucsmt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jllqqkwt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jynqcmev.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvlhfmzp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2moxprixl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qzunmkcq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rnksimbk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2piqhypva.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mmjmwsef.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzyxcbyw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2nnsuodex.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lypojtjj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ihljhttn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kdufpehj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dcgajjex.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2cvbxqyur.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cqwwybvy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogjsuijk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mfkhctfu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2nhzpekvx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uvbennmb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xmegrpfe.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yiuckcvo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eyoislco.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zbhtaquk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gicubssi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wwkyrazl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jtwfmehq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2iyicczfk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lmzsdzlj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yvsskpiy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xjvnawax.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ehnvgfvd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2anllkxjh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2rcgkbklv.html


<!-- 参考信息 -->