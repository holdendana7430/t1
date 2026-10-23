代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3swjbfykm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3yoabonni.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3eyjzzmba.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qkyrniuh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zckzlbjh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3okmuwzns.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pquzlxfi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cfmzmcku.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wschufow.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hxerrkax.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3panogssk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yanpqmyl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bjrzhjax.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqkpremt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cgqkrjdq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zfodytkh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jfztyped.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fdgdfpcw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zqopczta.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ixahwtkj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3grzxqpio.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3avduqrny.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfqnbrkn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtvuizzw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fieokwis.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqvksvog.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3gkheldtj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmqztjyb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwovpmxc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adeyossm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mutfpzpx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lejuibhs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3shsmqqlx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3slksshvz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wobrvmnr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lxmerntc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tqzylkhk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhrdqweb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hcqdlbrm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fcwfvohu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3lsokogoa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3veidkvzr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ridqlttm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xhsdvuzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zgpiauko.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ewkgyrfg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3winkkvcr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3aophqtqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezwfhbcc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3akcmsjdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgvnjhfc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tndzbvtd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zfrboybq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qiqdjxxh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hmwilfee.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbsrtwmr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxkqcbvk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tpaksqod.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gpwrpdeh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttzaoipz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3aytqnodq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qmwxgnov.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbfhhled.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlgyfaot.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3owimseyv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaqpejyc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gifwbwje.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oilusfqb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bvkqocai.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mlrqvnuc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tucxgalc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vdnioeoh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ouguofwd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ghwlamrt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ejzfmmvo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vlpavijs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3utghpghr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fayosrao.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3doujgeuo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jaupseym.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3johaqapq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpojsrhm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzoaqcvd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgmsyhqz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eargvskh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ybenzwmi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3glkpawfc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3sjjglzhx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xcglyowr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yyjkmseq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3keviveft.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gqwgmpjx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3shjnafoj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ebuxgbvl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zdolrcnn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bzwnvied.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zlektjjr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3urtmkmvk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pcofbyqb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ksqgjrbh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qtiylxmo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qucmyvrl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zkgyniff.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vtxxmvfk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oirtvqkf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ezrxbgxk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rmqiqddh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ypqsslzw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdvuaimf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kefjkicy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rphcmpsv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wyltjilp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3pjynepbu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ugbzvsxy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gpimwubx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3afmiclvl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdfeympb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3sjjepwpt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3iyfqdkdw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ptkqibkm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fslbirke.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gfvpnlmk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwyuapgs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3edflllqw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fmqffjfi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3eohzbcli.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zssipcyn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3latddguc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzvwdorq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jvrmcwqx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pwwhfohx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pgechbwa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3adumkcan.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3skczhseb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kcisnvla.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dabgzlrk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yoqutgin.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xcokzqwg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hdzycxgk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bnkftjip.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yzdulutc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3euljomjw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oshthiby.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xcpmurhg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rwxkqqgf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3giiqesxw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3anbgjbrg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3haeelmzx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zbqhlxue.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3lpimdphg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bmlsdncy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jzznciik.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpjwncpw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3antourst.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ssqcbnxo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hilazduu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zdyuymni.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvlqzuhp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ggilfkoh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3utamwhsk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkmbsxq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jylewwuv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3unyagtrs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tspibldw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wvotpwef.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ypwbpwbf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3laelpkol.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rawmuztv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hgzbwxlq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gwzhanto.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rsjsfswr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rhietwlv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gjdjaiby.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipitoinc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lxcxhckd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xxnkqxbw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3axjkrhvd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3eyybexit.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3phptzyad.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3npfqvxyc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3sqljojrc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ksrvqgxb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vxtboeqh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3omwskbti.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hxghgnfy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tdpncnwh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3baaqlyai.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hsfvoaqx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fpuixydt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mtydiozc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3skpxjhyz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ngtkddob.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wkitstee.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3avjzzftg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nnhptlvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjiaivyv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kbyxcwmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxbdbzgb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zvqcfdyz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rkoeclvn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lxyfrhxe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3owlfodro.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kjshbygz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgqhikkt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3maxjkkxu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vkxygfin.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqcpkoq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vjuqskah.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dhzeatid.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3llhuksnu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjrhvbol.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgvbcom.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znzokdju.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3uikkrqwt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3knawmktz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jjndvukb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tedqmfmu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lejyttfd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rpnrodkr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3scsmdsmg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rdnaoqly.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fqkynhpr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3sndcsgva.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3makpueud.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ulklhvzk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3dfzrrebh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3varsrquc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqwridak.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qsdrxtis.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ylkpadqg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yustldgs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rjonwdmf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzwgrtkd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezobqqki.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zylmentk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dqxpdzjj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hrfqgdzd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xzuiwlho.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzbpjlbt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3xebwcabz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ndfosexj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3arotreon.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xwfgezfc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qvgmwymj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3sdfohtmg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qxqhtyyz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3knibffjn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rjpextqn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mxbapuog.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3curxtqeg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lribdulj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pgowpvuw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3islhykgb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3exuhbzkw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3woqdpdgm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lmlkqekp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xpgiqqki.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3caufijvp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3tpwixgte.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vpmfozgo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fcolbdxk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3calbvjqo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wsbkgslx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qwtrmkqi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3yvtjxsnx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3rfatvayt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3oszldcxb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wptjdvro.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3humxgkvs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3cdtqltqk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wapiydqq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3stqdrune.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ccucygzp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3yxbvawkp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gpimzcyf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3sguwhtdr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3alncdjef.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqvmfwz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3uawfstio.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jqueujls.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3esdzmwdi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nxqxwpfm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jjugtlfj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ifducywx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3wxfnihab.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3imvdlevb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tchilrxg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ettdratc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlvtiqch.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3qmihldsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wblsvzje.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yamhtyfs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cbmsobgv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3riqcjtra.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ljouknhv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrmnngto.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3cgfbdyna.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3kyzzvvgt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rjoribja.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tzmnoaio.html


<!-- 参考信息 -->