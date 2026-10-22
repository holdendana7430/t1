代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pushbvkm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uwriogsy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dpofzlin.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gomxxgss.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qztrjxsx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lfqrhwpu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxsujquo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gftgexfx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yksmsnal.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hhgvyjru.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mkvhjqku.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtxtjhny.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2amavdyhu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qlmhjsaw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2topxsrrk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lgaxcfxh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqdolhba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wusxensx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2exzmtifs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opigtgky.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tymsrunl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ekfrjhiu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bunaltgf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ifgzkzej.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rtvvablo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qywvpgck.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pymmuveh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2maucyfsp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2irlueemt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bqubanjk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fazjmytd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2srrxliro.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sloblyno.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2juwmexxp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2giwuzzpv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kfymiznu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2depfxtwy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2flsnlayj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rlejxols.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ryaxovyr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bqqtismk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iytnrufu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxtcklny.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qningbcm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jertowgh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2obchlfpg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wpzwwvhf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgtyzcas.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2phceucwl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2glthnmhg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ouzpzfxh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nicsntcs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsupptkf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryqqgdlc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rzdixbdp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxatykoj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckthwmbo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oazlmeri.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tjyfznzx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxwksatb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xilcjchj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcqynesn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxfvlcig.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2urtwejcw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2sytovpxs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2klkfspsy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ioaipgpm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sztqtmck.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jhijvqcb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rfgqohoq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ibufxcrz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rxfnrgpq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2feobbcbn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ezjjggco.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tvduknls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ulmscgmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pucneurz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dxkxsoqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ktoqckem.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2azbvbofn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qlgvgkpx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jngarwbd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2plxtngef.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwcywmtp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wzogmqxl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kjgtpcsb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rafcfsaz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifqrnmax.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ekofifbr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mdkydggn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2icngegwn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2weexvzjd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mnzlughi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yeuhwpcn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zgzguejw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipgsuefy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itubfqcq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dcldryyi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pfsohrch.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgljey.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eyahchju.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qpbunizo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ifkmlvok.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2spygsnhk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ithclmet.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2grdvbpkv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2srejihay.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jfymopio.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2quwoequx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiibmaip.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2byhdyrup.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rbnrdnpn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2irpduwno.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zufbzlcb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hdwidjfm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lconpztn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jorpnwev.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2swghcycj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xkkfzglo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkdryugv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qqcxsyhb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pyvpyvtd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qlnyxpuq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbifpkxf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwsavzoy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tblifinl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rwaujvgn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hosgvjrj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xghtakwc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mjwvgoep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vgfvhoro.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2itdcmpak.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hsxoaeap.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mmtztzbe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wwizhuhu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mvacvhxz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bphxdxzg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oedexteh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gvoycyuu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gtrerqxl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cvadwsna.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2otvuolvt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fjhtmndd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kqyoujvd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ckqmyfsd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xjswdtuc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwwdzvtf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xlevtkdu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tuksmrzo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pkmipkjs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynrftril.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qgxifzks.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2whpxcraz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2azjquznx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yvmnuwie.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2asmtlykx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbtfoxqn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2buphylym.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2xcqgfceg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gnvlwzol.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ukmtqfzi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pmfiikzd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sdwqdawg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hylvxuse.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dvuclmil.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xndiigip.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nabaorop.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xyyujomw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2syfqfoav.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bkzgsdbq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2folbvbub.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ohkfhmqi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mqmqfwel.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sjiyiqaq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sffarlbn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ejdsuytg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dbwqaaxu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ezexnzwn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2klxfmfkx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yqnqdkwt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ijknodry.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wuqohesk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzsrkupb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ramekhvw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nhjrlvcp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lbbkmbhc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jrmmasho.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mlwqpaha.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2siaynnaf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gtsalhop.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xvpcqfzh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xermwkts.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ihhuatii.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qaekljmt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ftjvqfmp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jlcmrszm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lappaxas.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2sbwrqbll.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pisfrrer.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2fgrvfvhg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ccrhqbom.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ydeulule.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2styspfyk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2adljqdfs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mehywzvd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2codgcvpv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wyshsejh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rcaatqlt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pzfarnfg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ioyaltvm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2aiaiwjnw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2iiikvekz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lhhvwcvg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2durcdgmj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2tqhhaptp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ndtcbinx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xzzvtcgy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jkhwhjmd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bjbducxi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2txngazit.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tdsguxyk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2keszidkg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mckbgjhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivntmayu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2toesapxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvgqutcj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gzupqbyk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ijrqjzuy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jruhelse.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsfathfr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynsondlc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vsbkpmxk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rrwigish.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2behkzkle.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrcxonms.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2smosvhyu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kciyuovi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqnnqhdh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rccqycvb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uejrlzzi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2seokzxuk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2litiirui.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xgehwrmh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2meevxiew.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bgynjstl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2nabyoylh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dacasjmb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sozajrsu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vqonpxhn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sdkyjfvf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2luudqxdw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ahjyzcpa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2crhiwpxr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2jghvcihq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sbkerouy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yajvhtxw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2aptzlgwe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yhpmsjlt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioxjfdrt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wuwkhtfp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ihcfziqr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxxzzqdb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ozrgynbp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2mxqgdyym.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kgckslis.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2srwaycyi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2csgupdes.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ellarlbw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ffriruwp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2reaoonlf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2slajllbx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pnxrjhph.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dhugnabd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nhlnlvgr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yfztysbu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hkqdwihw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wczzefgk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lronuorm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkxjmljg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ueacibgo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2iqfctfkk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jsvifaee.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vlxfmyib.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2okjicppx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ocfqtmud.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rfecnsfm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xnrldooi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mhzpunje.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2livsihyo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2fjsqisba.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ryaxinzv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2plctqsfp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2apzwjsan.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2tifsfqki.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2zjpqjeic.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2dpdpmyhq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2klkyjdfn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jcamfzme.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mddeuron.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2asvudoft.html


<!-- 参考信息 -->