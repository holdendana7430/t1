代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ysknhujc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xwhsupub.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2czqbibcq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2aisvrlho.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bmnnnybh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yinuiddw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hzkcylfe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hdoruigt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gcdzninu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wxmronmr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uefzfjdc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pejkrkkn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqbwdzcq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vqttcfvc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jltvefew.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eteplkhu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrfekcky.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqtsxtut.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aliwhfwm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xjrdhcfx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfbnfzyb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fyvjisek.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xzolshmp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exktkdez.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jscubrbk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bgtaoqjb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2llzxksfr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bgmtesrz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rgmdijiv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jizebxlf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dmnxjvcp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mwasjxcr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nfubwsnk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xjztqqhm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ahjhdvgq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2eozgnhdc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tfwnsvwh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2urejfpty.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lqblworh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jvdquatg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gpscaxjc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2btcjeqqu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tlegpkgx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2iomnnwzo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nsogogsm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxeoduvj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gedvttuw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qfxahbkf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tnznotgp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yqhnvbbx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2muodhlfo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzfxrblp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xkzdfuph.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mwnmwpyl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcmcbgsj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ixzfcxsk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdzxxupt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsezoukk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ulegdvqu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2egevtklt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qckivdpz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbajbtae.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkelezlo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzzqzchh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kqgbgwhj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rynezofk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2klsoychw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jzzntzon.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hwbgecee.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkkxgeua.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ubydylii.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2spvlcibw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xuodpxct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ysdmfmbf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ndemcdfo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mvafaqlv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cvawfxhf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ipjdafdu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nqgwzlvy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jomnfrnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syybhhmc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wsodnixr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtvdmqcm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sjfxkbnd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ieazzghm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2liqzqayp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mmvyzwzu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jwqlpfjh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jmqbicsv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kfcyymca.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgkkoqqa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2divmntaq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aefwbnpz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2famgbfdt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2blgbsjcy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ungjawwc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aixzgcmi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2varmvnyl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pktvndoz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qtleptzj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idbdzpmj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hsnabzfx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2imsuphkw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ihugprdz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oshbtath.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2huxlzwus.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xtwcgsph.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2iuwayijg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jwycguiw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yzvwxnkm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2slnewlhm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oehbljko.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aodyulzb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2roelpitg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2exjkdevu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yltkwyco.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lvuewubp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2goxygwez.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cyahmvou.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nryjsine.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vfjvbowr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cookrewu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruggkzzw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypqjhhyh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etvmbpyg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2uomuokly.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wefwktbg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqhdyncf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oiavnawd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qfqsagth.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvmmvkls.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrrkgoau.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fqfgjpte.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vtmwbype.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vpvuuapr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2tphyrsfm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2saenwngi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hqvolewt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zygyillw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2opqjaihd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2afvytdss.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oqopinah.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hvyusidk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2msqsyspd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ahmcrmfn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2oobtnlje.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fzhrkfos.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cbsuuwtt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hdjjqzdh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2opzmxtca.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2agkpjvoz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ipljftve.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jtrqzavh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2taexptuh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xuhhlbce.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bmhdnxkp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vtckhruh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zlijjank.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ggqckybl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyorbmfz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ypkrfham.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2podybsei.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zzlfgzhe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ipqmcjdr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jqcbfcid.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2dmzjkgir.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aevwjnjq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qhlnzddi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ipmywhli.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pnoutrgj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lsqynbjd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bcpnexbk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tflremba.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fzmetncx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zrzemuha.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dscbnmte.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hwfwxhra.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwcywhxi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dhzenkqp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vxsirxzq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2etmdhvmz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zimujxeq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2joumlznv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2frjpkbqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypglsgri.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lshhaznw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llahcdxc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkbcwfth.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zxghhppd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylhtvdoq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2puckxvlj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2siaxpttl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pkflcsis.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sersnmpf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iymeqccq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2boudparp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mibvxmdt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nejqtaht.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxqqxgy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mtuqaxnr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jpdimzgw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2clkvopzr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kkwzztmm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lnmocwil.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jgbrbbtm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zdindrjl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bgavsjvz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2uaamrmbi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2lsgnvecl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vzsdwtmz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rthzdjoy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrwsepyt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ywqmsntx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vgjzafqc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yjbcbkac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2uvlwvpqt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2elcttpbz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fawxdzef.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2alkulhgt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2aexgfaee.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rexwoogq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jtzdgjzt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kjnmjqhv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2mvjnpmzl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2anoqktfr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tkajnmoz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tonyepwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tyxwaoat.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2naawdlix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2totawfvz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2teeogxao.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2uyxwapzd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdfsschl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ncrtwcjl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqwoyrbp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihcdjbmt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2nefazoif.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jyntasmm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mswrcrra.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ygljthmg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uvjrvdhh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cekdwhcw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpvxduck.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xkxmthzi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wldkoqoc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xqtdoxqf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fnslvoqm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ukrhfwep.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zwpwridr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2oygaphjx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rgbziyzz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tiudmbfe.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xbcgbavd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kmbvalxk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2yrwctxce.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ecbwgydx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2achzhakh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vefprftg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fwpjkpla.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pgukydlt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fhegyvak.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hbxjrqpd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2brytroix.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lxxukbse.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2pdfhgpks.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwnhcuxt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pfdkgdat.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nscsuxzo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ucnabocw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqyyuwxl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zbxflbnc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pctsfooa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2yocwsisd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2kmpfyqea.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qruzewkt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xrhsanid.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2tklpatul.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ndzxbbal.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qcyxjrjv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hqafroyx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kxvcjzmq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lwjdywbe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vwzqvkop.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lxqruomz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lgkxcynx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qlbulwed.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zsxbtqfp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jbnphdfy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qmrrkxyp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fdiutdsi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2pxjixcvn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2brwfhxbn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwoonvmb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gchwxfcd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wkfjdvlc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2xevtvild.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2rnrebutd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vsqkxflh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zvptymwd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qfjehnhb.html


<!-- 参考信息 -->