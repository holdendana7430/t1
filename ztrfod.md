代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ihyeuqyg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mtfztqaz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wvkgtgpv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2utrajlyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tlqoznhq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eiphrhzj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qfmjmfcu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nsedhgat.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wxdhwsli.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2euqcljiv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kjnxsipb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2focpfhgv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tgzaadqr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xuluqwqg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ittmfruu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dpeqtcyx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cfpewory.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hzvrljid.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bsvokwgq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vnvessxa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmkresxt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hhflstaz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2krwngsoe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvelvtan.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcnumdui.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hnlpkwcq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdxqjtyo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2haolrrop.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfqvxuwm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdxqjguf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ftfgzelb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdbnilc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nmmttfoi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zbjcwbpb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fwwnvpqz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yecbjrwl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qxniaczc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yyjpvaqh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2llwfvics.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gumlexpz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2iqztaqfe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ipktgfrf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qiywyutw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rpvnlfma.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yqucrmcq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hsyjbqyc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mzzmcczl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jrkwrbvt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2voxubaao.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yyvufayo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hlgtzeop.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hcsgbqhv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ddmhsmqp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxabdnjy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oxuipclf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nhwodfyv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rdlmnoge.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2whyneyoo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ehuauzgz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acjfakzh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tmiiujki.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xhwssmew.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwztldts.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2prgsocvo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbdvrayc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktvsicdk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sraqfdnh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqxmooje.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxyifnzq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbhfvrpb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ngkhdmix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvaukzax.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zswjfxeq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfdofrzg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgxognvx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oftmzcce.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hzbgugnz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnphnxhz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2seibsdsa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pgtvoqyt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gihgqaol.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ywuvxeml.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2aaddijdv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aqpzqfmx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pfpukwop.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2yjrwxtvl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qjxhfnot.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ohouehgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqdobncu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xufrxyrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2faxzlqaj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2iqjudwvd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2eykermnl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2latwgccx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zwrlfbpb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipouvxdx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2invazrfo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ebzdqbhh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wakpobmo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wmlbentv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zigimkwg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ylbjwacy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmxxenmy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydgfizli.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjnemlyk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvysmjmb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jzucqarm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jegsrszk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kflsmvpi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2omzhmpqb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dfkiejzj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qkxhhhph.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zcozaxrz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kecezulh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eqkprbfj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2yzqumvli.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pxhnylts.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jdevunbv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xmbcuutp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xdhyrcao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mkxmgqon.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lqchitbr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ztdisosl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgmjvnuc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xnsaysig.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lbkechib.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dnseqbso.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2alsuopgd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nwzddsbs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kozoukvh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zurvzfqv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkojdfug.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygodmpll.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2oqsfbrjy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kttxjtue.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yvxuntkh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2reggybxq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vzgwkxil.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqcbnoqh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqyhtfo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dfohnfgv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnurglmh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2eqzbkwce.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpaicpes.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uuimkvnw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hsstgamm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hzirzvns.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xdesjkuw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2izstylul.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ogndsgxk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2leisdhws.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2aysqkeyv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rgpkxeyo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oiybqgyk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2olhnogfg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2drhktlzf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ncybdkyq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixfekmxy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dkeutuhi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lyqavtef.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xjiijchj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtcaefgr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgpljgce.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rvivhyek.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dodguizc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykkmayol.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bpmmyeei.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpabolqj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rzwziezd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zwasridp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ilpcadga.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnokoucw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mjeznqci.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2kqetvmmf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vmoqkjnd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2crerseuq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qycvjlom.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lxcumxyy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ivcnlqdj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fvwatzvv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rfqtvlhw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gflywobv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2iutkqgin.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cszekosx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gpxsidmd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewsutabs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dtveaksk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqlnqhm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2usbhjthk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hinmxzdj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fpphvwcv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kwdwcnda.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kaocxnuv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtahvnga.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2voupnhip.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2icurqcko.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xtfybuzc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vzgureom.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cnozmnew.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2defehdiq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pomzjhur.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uvhhxnvq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eyeaxymw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nrjzamnn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oyzovsqa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qckymawf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2uylktndc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nbpdafpj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vlwdcqhw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mvxbmoms.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fiaiwaby.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hnugtizp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mcaetizz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zzopnyaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xgeidngv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nieeeaps.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2efjiwkqg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xwqymgvk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rshndsve.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2befcgixm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2nlfadylo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dfgpiuom.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vbvrdyur.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qibgtens.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yfzhsmks.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gflgajge.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2oiqgvcma.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qohgcmdd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pkjrhsrm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2scbmwmqe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ssvkxgsz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pjzgjnuz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sfquvudy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jotvhvxa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rnxilypb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htevczda.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pcagwvtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugetiidt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lzkxkmwi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2clqniacm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaneeqzg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eeqzgfti.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndxliwwl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nddmkfpv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ngnirgkw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2drtuwwys.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kimypvbo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wptyefws.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ownfxfhy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjtkgteb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yjhnaekz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tvswgjfw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ebjnbunt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rayvlsgu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxzfmoki.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pljeyuws.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bsfemjnb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qmbcpesj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wueixpsx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qyjsiybk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hrtnzrpz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mfgrsnug.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vihdkwax.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bqwdqwwb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wrqizins.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kgutkrbr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rbmtylnw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gycxttcg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dqqsojly.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pyofscva.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjbaycgy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nkdiqest.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtbrfiwq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pnhgvlud.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uvvwtsid.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ejhlfwkh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ujiasazn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqqxblvy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xoqkbame.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzdxvcjo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kaslktya.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2eraxlqhh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2utgptxmp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cydqnpjp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2uvotmbyg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fwpqsyno.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cwakkiep.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fqmrkvhu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbmtbng.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2frqrbsde.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpqrknkq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wadmumhh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tdsdzdlx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ialccwbf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zqowpqjm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oaxczgnj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swvwqyej.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tvoqbfpk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xyltpbmc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fvjngjgj.html


<!-- 参考信息 -->