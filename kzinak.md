代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsiuibkj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jduqmswf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2glaaytqt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2znyulsjw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwrddqsi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghlzsduk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjztfgtx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dsfevaxc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrqljamt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brsvzddn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2aavlnytl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bfxzlkcl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pprrrlhd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uinqkiad.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ctfbqusq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2obkxztkl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hiywraxu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gfrnsguz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bnwlbmnj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xnduvnbq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vihttydd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhnovbrg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ipvcptwg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xhjddyks.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oxuksgnw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2erkslqoy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jgnhqwzu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xbbgqxjn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wfynuqso.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iavilege.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2btjpnagc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nrdktrwx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2inpgqssu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ppowlqjs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wepjbzjy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjacvuix.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dyvznmso.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2njcdalmj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbqfhpiy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujkrfvtm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btghogcr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wchvpnnp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2agkmsxjf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evwjizja.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbdhyipz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txakzhge.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ncqzbuuq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwdctkw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rxrdgrqd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eddyoqmj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2auqdibvq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2egrwsbwb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fialzwta.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhzmurbm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nbzwagki.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zetjmhhz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uqftuviw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wwuxcdyg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jmpnkgqr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lmhsyvpk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ohongeph.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2aiiwrsby.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hgguqqhy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2iuvsbduk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzlclzcs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2abpupkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bydgskxn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gbeuwzea.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ltobocwc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgjkgbue.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ussmjqqo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pwcaufdq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pqvklqgd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zfhoavfk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2acsdntbt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2almejwzb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pcydagdv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yvtxlftk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nwvitfqn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arvuxexw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2eakaejel.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzjsafrb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ylfypowi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikimdflo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zfvphqnh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2eeszezxj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zvouymll.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jsevjtpl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2omdatrgf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ifzufyap.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uquclzyh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2evrogkag.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lcwagkyd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eevfzqtm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2osvfkwyr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kdxqwxcx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zavjhjqv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2exuhvbrg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bcmjszan.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofvjevie.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vifqdjoc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jrzmkupi.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2avhpkpxo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2leeyzwhq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2spmomsii.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tggolaid.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mksfjbsz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iiyllvlt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rzaigabw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qadcubtq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqglooor.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nrdouypn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qbztjnsw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xhrxyalz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ikmfeatz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjiksvk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2omjrgvlc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwjvurmf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2iwbaoldu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fblhhnbe.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kxsjvtbn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xgnpytnz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2soygzwly.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aioujzet.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zuvxmxlk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fckykwbi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vwjvbumj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fvmjxblu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2pmazooef.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yczdfrul.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zsgjsfco.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2trgvgtvw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkzqghlf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2stibagyz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xnlpwxnm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xcwtramr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tlivjwux.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wtvfnesm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2msjqwnep.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bqesvxpe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pkpmrfzt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fdtkyhvs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xpwpktsk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iagdqqfl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zrykiolm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2yybskqvt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lhmklthu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwjrsqaq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2peypinmc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2skolvkzp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sjoyqoak.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sykichxa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dyzgyopn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cahafmks.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tjamakjx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fwhabokb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2idxjhgej.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fmyfokbs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xnzuyura.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hxmujmrk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rqpzefpv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xsknkhto.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hstxizso.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vkvvjjzd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qrstmsmy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zllrcbru.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2nlwgxmpt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qaynbkzb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vblllshs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpijykas.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lneothvl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qnkvqngq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eamrnqsq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfknzqxy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2opibpbcu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vueumhct.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zglaakso.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fnnpumkq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vpqwfcjt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fxfundfd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ptbltkgs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nwpslasr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2lskgyxst.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2teyjrulx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gumjfplz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2icelhigc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kugohawo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ijncwopu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vjqvxapr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2esgjncqe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tqgwnqam.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wkmhvadc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xxqwkftd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jfnaalxn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vtqnylpf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaacucsv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ofijsjxz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eclstmds.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fsyimfzb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2omljcmcf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2utixishz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ypexeymj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2bvwnebgr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2uplikysw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2yerjuhgr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ogndglko.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zutprkzb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tmwdvohz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dgjkplwp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2adcaixft.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kqzwlgzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbfmceen.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nsnfdbmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpriwtcx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2estmhbxe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yzsldlep.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcarxro.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmgcjuph.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zwbcjsrf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hqociprx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2upzjjtrd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ngnhmwwg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjsatker.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lmalecwg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hnbbptey.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rihrnadd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2makxsbsx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxzwzlt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yjpqitcm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yzhnmuar.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dwqvnbpp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2scosbthw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fomirdaf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bsbyykpb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kgdqtwrf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xwkgavox.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mtcsyxep.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qgqxynld.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2zlitqney.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vkjeebmn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sqtsfdau.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tekuodeb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2iudkmqaz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzcovczl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dujrbomy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2srllalyl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzdkeyqp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zinjfiub.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hxcgnpvt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixhagddy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tzilrvmq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zxtmjkja.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2tplrkrya.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjmnckum.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nhcxrpfd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2adgcjwui.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wppzbosw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oygdtjbx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkcouzgx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2mpaktaho.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sxtnzadl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nqbxkslb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ifwnyycq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2duooqokx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqcmfky.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kdjoarvg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rylprcyf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hnzlqsfp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hfjpghbh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ggngvsev.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vkqreiqr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zlbdhctj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gqjwsrhb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gsupeztv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2idihctja.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2jxfxamko.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pfagzjgt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ecwzoafa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mpwnflvw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2eajriwei.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2smfkonad.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ozvqzpbm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bvzavcje.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ephkcvka.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jlzofail.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2bytrwhgq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wtagovng.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2teqjmiut.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2uzxehwkp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wihggffj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ubxfalme.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2texngtsp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2fkrqtaym.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpyhqkg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fxvwocmb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rwjhshfq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mdciwybk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zjisxxmm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2sshbkwmm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ktjclxtx.html


<!-- 参考信息 -->