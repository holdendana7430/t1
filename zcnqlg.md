代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urljlwxq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kncwbumk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ryzgwhnr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkxgqkbn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpkuzxkc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uvtbevvf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2eeglhank.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2djkyxgcn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yoograho.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xzphkpox.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ujtgqzwh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lowburga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xbwpyaol.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wmcuqgto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rkvbsmby.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rdhptffs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wxqasvhi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjlnvyeo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zawzktxh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zhphirig.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jyssrqka.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2sqvqpgea.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bpegeliz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sduurwnv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ssutemzg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flgazwcp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2upjgxcwq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xudjgczb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oqcthkvb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fmwosfup.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zjbkowno.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2siohmbxh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ffrezroe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rhcbgejg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xymzrpbp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avdsrkpu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpxifmja.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwvjkfid.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zcdfohgo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oleruhvz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cigfrrrx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfsbktpm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vlbeinpl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtxevmji.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vpwuhsbv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtnfmjtr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yuibzgvp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2exacwqci.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jdkjvszo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjpvezvo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2sogxdmpi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fduxxqfw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lgsvafho.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pnlyijdz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qenychsj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ikppxypr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2azamsuyu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2allvvfxm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ixvsltgt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yugweioi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpuujkzp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mhphdaun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayagrqxb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lgaphmxs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vgsxjrjr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ppjmsspi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngembqlf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2simxvggc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ouxczuvh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2longlxzi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpmzqplv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2reieozbk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2msbcpzkt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2inimmder.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ekidrilt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cowypkgm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ikbauphu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2prehkvkp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zogmwwdz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uayngxsu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bbevbzwd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ybfmfwup.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zpiaehwt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zpdwxbyg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rqyxllol.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yprnyijd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2arrkwirt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hbzuiddi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wfmvrtpl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2snpgqnpd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2taofjnkq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rrcdvcvd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2peauyten.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcvvwrlf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xztflkyb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tvkameuv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kwuedezf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kvufsyjk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2arigynne.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ulrfeybh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zquikmab.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbtharts.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nxfkniks.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgmfuwep.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2drmhigbq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mflaqtko.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ohndqfki.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzcfwywx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vpcvlhpq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ceziucpw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzxbuemm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2prsrnptn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eezhfhqv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wzpkfzsb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2giydvgjg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2csrmodhw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xjlnrygv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mutzpguu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ymjostpc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2soiprpcj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ewxffkny.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hhlirosc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2itncjkoc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nepsjyta.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ctmtjtqb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wfxrpain.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2geiavbbp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2pulmkehe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qrhupiog.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xeityrfh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfybuqqj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uhafbvmc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jkfrzgrh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xeuswcga.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2czvdyorg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lgfoccic.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xdnryzkr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jlgxkszp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zavgkmfz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vqchfvfa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ywdxdjar.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cjervrlp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvuujhlg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ytfovzfh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jykesbyv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vslelohb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bxwonxvm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gozwzicl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ugrxdfwc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ocdfomsc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rhpumqwb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ercnprol.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bmpdfkoq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bizuljqc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2sxebdhhd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lzkdupzl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uukrkusz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgrsmikb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ejfzcsew.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2crqgvfux.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bndrzpjn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2povddecm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2gglvpbcw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cwyxlsbl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnqsisqx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dcznqpco.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kibjlzdp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2edkvwzeu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lqlwrhyw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jjbnbcpr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xmbrqayu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2thqtnsyz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vujfdqbk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rrchpvic.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rklimvry.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mfchiich.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2agghlzyv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2urqdpdsr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hnjppftk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ktvvcqgz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2aileitpu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2sauzyklu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ukdvcgmn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ypqlmfzo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2imvmyhgp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vnwxsyjp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jszjooul.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ednuhpbs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2thoxpcql.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hwgggcgi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2inznyull.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rwetbaly.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yrzqjogm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uxobaids.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vvbtpssj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2glgiqony.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bgwsmbpw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ywctgtcr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bbgtexmw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xrvnhsfu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nqkppidq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uawmfisq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubinytjt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gosrzdvr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qzzzkpwd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xmspwjlj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jpfwqrnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hpwlitkr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sxhvpgch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdjkuqin.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hrpnpxmp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xxohcmqf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfcqudfa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhzohdor.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wepzajdn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2sywxdjhe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hskivysw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wgtxkwvt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmpysjwr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2iytdqski.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fexgernm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmmkeaif.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mswhzsxr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2grntvbel.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ngxlqrqa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dxwuzybe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2woyfazrk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcxuqydz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tzmcykrc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dwcofmdq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yjnymndh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wtypbugi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fdmpwvyg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iiwovnfw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2utojtwna.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2visetajg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ozhyafri.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vnukgopj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2daevvmwi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kktkomsw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fkmwxbey.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2trrgemlu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eatbqfpb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hoygrdmj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjlbkgsn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pijxrqss.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pirgzvjj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xgkhzdww.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2aarxtdmd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dkrfpost.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqjqcq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwxhyorr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uycfnkwc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2igosiflr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbhsasnp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2auaztstg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2oaketbzv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ricqrgjk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sxusdmwj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2eqvtryar.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mlicejbp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2spcezbrm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkjezppi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dqsblsxn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mparfgiw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jpajvbny.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2olmxzddw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ampqcfuf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oqrwpztv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zhgokwzz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2amcoguew.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2cgwmfedx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dqhqfute.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2iiankzhd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mgkininc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rwqeimlc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fwsfigiu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ftswxwkh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xjrrsvtb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gnhwsvyz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ecdwnspm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2iakbttqp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vqrbfbsc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dpfwnysd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tzbjomjc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rxneudtd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lmjlhlgk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxadxwb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2oypcblhr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tftrxzmv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tsjaoyni.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fldgsogz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2flvqdpis.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmaydc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2makyfvrn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uzkdclpo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ntqsbmpq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2vhombniu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ibjvcpbl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wbpfrxyq.html


<!-- 参考信息 -->