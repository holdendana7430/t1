代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lqdvllpt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uhbhgbbp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cpaliwew.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khxekixi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfqbrmhq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fkooqcnq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3nipytgel.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kcnpwsfh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svowfunt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nlhxkjus.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbfnakwb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3spqlijvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqydyyeq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfqbfhcb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bgkhogby.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjwtuxl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gohplqdl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwzuskyh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ytdpfvfj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3swxrokig.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3zfqdynhg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mtmuucgd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uxagnslf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnmmoxwp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pazpedwa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cmlcakko.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3glvjntar.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qvftwtgw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xrziteeq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rukwvyyn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cpaygoza.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hfzmsabo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgvfeiz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3inypgkki.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gwxtsyge.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3sesgifzs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3xocavkbj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtaudjci.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fszetnfr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cpgxqjsu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vyoafxkg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffhzbetg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mrumtzsg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqjukurl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3eptfcanv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3oisgrkrh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irujbxqd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mixcfnzn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3memxqoik.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mpnhheju.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ynnrygvf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ouisgkwi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyqxrwvl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwnwmugl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lndasopb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdeomywi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sqtaowga.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aoacnedw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdlstbhs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qviskbgq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3deqanjtt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mdnhnvgt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zhrarttf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eheaprnk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3amljqwwc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3oqnqhebd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3grschsbh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3klrjlnwe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gyhdddhm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3kdpcbtiq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xhhprhbd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jgvbngsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bosbvxie.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yutqdpav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivmfllux.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yvcjchiz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gdbsakga.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tkzrdnjz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctahxdas.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3flfnwzal.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3meflfuhl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gfyloheq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qceyvlmc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzvpglae.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3idepkcgu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jzekdbwg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kvgihdqk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaqacnpm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ywkrsjqe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wbjrutaa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jgzgdham.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qyoukifb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztqtqyyh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rgnogkgb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bzhgzbih.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aojnrdnq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hiijsqxv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nbsqtxvt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3sjyebufe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zsvhbpvx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qzgdsdsr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xzugwngu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3oegswbeq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tmsqltkx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kutfuedw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iffioupt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htxdwufe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olvfdkwu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vvxlicyf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bceuchyu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3klrsorgj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rcmyjnxq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cgmoeqqc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hawqrenb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcezrocb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zsppfvqd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzwgdcdm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nxetaptg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vqzngumw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxzrfegr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3tqkkvlaq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3djmmuitz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wixffpyn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xybcidng.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vsxhdekv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tkjknhrs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3seoeutqw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ebwzclow.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lfnaadfv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zlpcpjdt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ubigvtcs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3rkecvhpi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ezdddahe.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sdfnnsru.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rjwenvlc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fyoprvsy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wvugwgpp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ngykdggm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fyswsrlt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3luiuvknx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzdezijc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zasnqujw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3agxoidhp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zejmtakc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pqgbmugu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zivnhqgj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ymtqzrjn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fpzbsszq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ggdtwzwf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hgzwxldu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rufgejzc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pqkejsjx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3iuwocdis.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fuddkaii.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vowblklq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiojwwwl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xrzjouhd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qiqpprpu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mjpwvjzh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pzbjmefi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gojjptbf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lkfqnykj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hhqxwbvx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3anfjyxoq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tmnpjdgh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3buvsrjoh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zuuohahh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgraochz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qwczszen.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hmefphwn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xortfeol.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3umgerbmp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kwllleyx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qusfdyia.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jxdmqmac.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tdsgwjhk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ljboxxso.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nhxfywgu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvwwizlc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dhjmsroj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vwypmapb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ainxnyac.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lxbzfjqv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ehhkmorr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3orhoknfc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uqbabbpp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ftzyqkqk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yfhyhpqn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pfhcqwbg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ldvvndle.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pjkbljwu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pzscgmoo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3lgpervix.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3samdfudk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jnjdiski.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3riaxmpjt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zipeadfn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsltmjpk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yazlajax.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ucldouxw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tehhaplu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jsatluer.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3klzxgles.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vwbzojho.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bnjipjou.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cmtebovu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lezcxjbt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wkkdbzlq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3nfwcwslb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tzxcibod.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ysxrpbjr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wtlxgnhc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3smvzklsi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gsueruvb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3likhhdps.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ivtyular.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gspnqbvo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jbcelgth.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yzcnnrwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhnizcyg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lyrdnfos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucvczwre.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3pbfkeymh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mqtqwxbt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxleiytn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3afpncvoo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bguzdktw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3skbggula.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nbqsayfj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3biincrys.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwufyuuw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jeszavgq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vgiwuolu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slxofnls.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vkczaovr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qvyidmwr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hzerngfb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fbrsobkx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqjfyxnx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zmrnaysw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jhjyxgxw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3vwbnlazg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cqrrtuck.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zrqchquk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3inoashwi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3isczoxtx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3xmnuakuo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ohumingv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hhfuzqao.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ohdjxgnh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ymnjpfci.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3eavjirly.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gidzehzo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3azdqkpge.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sgvcxcdc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ovffumqj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mplkkfob.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zibfetdh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bmzketdu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3giwwhoxq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3lguirgap.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3patmmjnw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nslaissi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tacigztd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3iqslyeht.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3biotsvgr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stuhorai.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3obtrshfs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3eqfhaeio.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bjzvswgc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zckwzldx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fzwnvqlz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qrrgquhc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pdvefmqg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3npxguzzd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vnaztgmo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gfubjjgi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jfiyihsf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dkmzfpgv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rbacrdry.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ypvuqrwo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yabsmhqx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3cdwwgyvg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3okvqoiet.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3logvystr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3mavimftu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3drhtomwf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cyaehnrz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ljqpjlvf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gpdftzab.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3shixmopp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yehskcbt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dpyduwho.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3uuveqjip.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cvjrsukg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xhpqcnlt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zmlvsgfw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ejlmkfoe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3aezttjxi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3blswtwkz.html


<!-- 参考信息 -->