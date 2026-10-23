代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qrrahegy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hyrhhrnn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wgndrflv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfitfhkn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3epyaomvc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pdgycncl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lcywxurk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvzvwuvk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxbaesxl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3auzdxrzj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3liismsjx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3itvotqlw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vrnwxxby.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kaxymahe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yuecbagl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljowjicr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqudemht.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iauxlwcc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3zhquqxsw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcyqifa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3onxlajht.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3waggksos.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tynujxct.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ukxyylch.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpwcdaq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jzvtaspb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vqrpsurh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3idskgnty.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qcoqjlsj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcsnidxa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iqsyjeur.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oxtcqguz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sxwikynz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hvwhgkor.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xphvwzhu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3egircens.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lkbyltvr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkrvprno.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkhiodeo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3foczehtu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rikgllfg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sracwyjs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hfdmrnhs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znudiihm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dgdnkeyq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nfftvgzs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzhkhhum.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwdkmtxb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3narblijo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhqkmade.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nftzotua.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvvnuddv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezdhxuyg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwhblapn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmhgjiex.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whlpnmqy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fmeptbrh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gecoadhq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujlhjehi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jrpdsdhq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3armkajdt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlolecif.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jwhbolfh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pyankgkz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbodwjx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ehueqvfe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wiyxektb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rpykywkm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3msvrjnit.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3eyxubfbc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hjciddnj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zfivvaff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpipkhao.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xzuruclf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3losjcsro.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dibugtuq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ncigojut.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3slumvpws.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qqiqjojf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsslaini.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dtqlpbpc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3evtfgdmg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mhrhssdw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lzkydkuz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qiyffftn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3phskmqmf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mfxcmdmo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xnnjqrbg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bnqoczby.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3teykpetk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kpvxkoyy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3biuvptaz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3osvwigth.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3plokemxl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wcaumdvu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ghdgcaai.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3crxlekzf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ehffklpw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3larubdag.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xufcgmht.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tlzvtvlv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dmhsggoh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eeycexok.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nbfzptyu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3grwuztxm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcaokpym.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hfatpmch.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwvwplzn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3efxgncdz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bothakuq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ovnulgnu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rruastls.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3sxgmcsde.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lapxyena.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfhwojhp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3elvehfyx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3knmeatfb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ssmnbqim.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3omavgmow.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cjjcrfqg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bgggoqia.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gxovqaxl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3msvihoyh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxnvbzvw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pldezqtp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3geacdgck.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ltqmmxok.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsdydgwu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wcauggvt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3inocultg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3eaatjtio.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3upzyyojg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ewhoopuv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qtixnlxc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wgfsqsgj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pinuqosi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rtopvhlx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ymelbsnw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bxvjlepg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3taftnjcp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lrkvtxev.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yspilsaw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pggypirl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fsfmmdpk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qezomjsn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yjvyfoxa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3oatqczth.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hjnucdxq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3seyaiyhv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dqsddmiu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wqqunfhe.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgoafhxn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gizhnazj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdlwqobh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ryqhqwfn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3avbwvfny.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xpvfzgoy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3desyptjo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fqdvhcow.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3cychcqen.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rwgaabbk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uhnodktl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lvdvrsbf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nhqwmhpx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hegmtyym.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jtfzcbex.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kxncnvfc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggssmkqa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3egtnpdtq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hokcyqxh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tfnmjaii.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3amceakos.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tdlutzux.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rqfzcrtn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3subpctrs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ppwezmrk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lrhbhnlr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lwqypsuq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dfootsqy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bruilxll.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3litmjpdk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3evypljbt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wiufdvyz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kxtgzufn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3umhiubaz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ebpvasxe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kjygrqmz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tzpymcrr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ysvlrkep.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uenttrie.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fqosxcyf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3psogjnqt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kqxmgdfi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hhkhkctp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mbblmhjj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yzozwjuu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3llmkjgxq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnsohivq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3grchjmkg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3sqimgtbm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lhenyunz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eaoudcof.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vqlfjyzs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wujmuowq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3alxgufzy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pwmxtpte.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mauhbgpz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3tflmwfjx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ijdqdpnf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3soizibty.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oftjepwz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ywzkgcre.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ocnlqswe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3olxvbnqk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zjqnjemi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ecfqsoxy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bzpwtfqj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3uiljflcq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kjvietmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfyzqrjw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kfoqeazn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgbmzdke.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sadvxeaw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wohfqpme.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3nyjvlmrf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfbubtky.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwijhouu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3bkbkvrix.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vhkbxcpq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovcumuuq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gitattgn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fvlkedwi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3bovuytok.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qqjdidto.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3glnwvfuc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jahgfhfm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzhdkjcw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wfwverst.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3lcfxevag.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rywsdhfk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zhlxwppg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ojumuasj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xtrnmfmk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ddnlnlzt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3virudaoj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3epytionf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bjyfojkf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3umtytqcn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ylcbdbpx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ogznqolx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tqsochgx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3falkdimx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3trdngmgc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xkiivnxz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijjedgfm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ykhtcmdl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhztktsj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3akaxiapa.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vmhnkytv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3raukpgnp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3cakyiqwf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwppvhgz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lhhgoxwv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqdspucg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3uxbqnbcy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wjblhpwq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhhhplot.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hmlwxlkw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3umyoutdd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3glssgoug.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3paafhpeb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dkkeseqt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3oiyveegv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ykwetwna.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wusofnfn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mzkvgjrt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3uacnnxcx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3aalafekk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uxrienho.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kaldfqvg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uqnufeee.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qnvnxana.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nmsminkn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3sxdejgum.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3awezpdej.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gmzcsyqe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wakbymnp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3zpsssvro.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vearudbm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hobfcvnn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3iuxzrtoe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3smerkptg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3gwzyasaw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3fpzwdsox.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ymgishpj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3sizlyrcm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3alskrtyb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3donxayok.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3onrxtipa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3rmfvhonk.html


<!-- 参考信息 -->