代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3uvhnwcym.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ewaiupxx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqflfhqt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nsqakolm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dezhfowx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fnildxqh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ecxifybz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kebhkbwf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcanvecj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtklmcmt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxodudzf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzbrlcrw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ayufmjnu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnornffm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxlmzfpc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3smrkgrub.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gatcbuzd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3apvluogz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3tshlfnxp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rdfdpwvj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3blvwfvxs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ojowvoik.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qwcvckla.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pdcesmqu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jlszuisk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vypaxzgs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wqyorsec.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3oxychmpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbsqbbbo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vyldujhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prhjojcc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lkgrxjuv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dctqgzzw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hciejloq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsqeiyll.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3erifdwte.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mkcphkoo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zuvsonew.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghkhzzvs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3njtegpbf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nxwsjgyt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cwxenamg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsivxvvl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3euxujyzd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fchujfdy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uvhyrocp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kxzohkso.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ufsbsbym.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htoitikp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vfybcsut.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3egqsuygg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nuzvpoyp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vvhbpqmu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3kounlxtv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ygypdztj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jwhwmbbo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bfhvmbod.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tfuwxnjc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3efydxqus.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rureotum.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbezjicf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmjbtbrl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfwhwvnr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tjynsgoz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iayeuoco.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bizxnidl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ezrasjec.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ynhlbzpj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3asydaiin.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cbkpqhlc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtakqmeg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tnetebje.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3umabqfgc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cdybvfxd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eoavlmrr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsfapuau.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ibflenub.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tzfdlxhf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lnnjnhws.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3krbicrzu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ezkvqfcb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wpahyugc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hcjhduyr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3whtggnxa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3txmsxilb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tckhfewl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iybuvsbv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fpbohwyi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gqlqxehz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xrqpcuki.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rzoggixv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lhhabwjs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ysmbgyel.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3alvlhkdi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pbnjncgy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yxcsjfkl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ojzvwjti.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyvcgovo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgokmuii.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouwibczp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jbkepetb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lscqomxo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vsqrshtt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hkkjkvod.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ydyhordp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgzpqymv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xsdbgykv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mltvofpu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vearxcdt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3tmfmrmzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jmfsqwrh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikitddeu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nogehvlv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rsigxqfe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3flxumbny.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qrykuwka.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fdygfojk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3llhdpcib.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nojxuyrt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lnsxgqxv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hlnvmffm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dvfyvbii.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pdonbhew.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqscxdfb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeuorlne.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njsjwyer.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqndwwcb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lbrojgmm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iplvjube.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbsvnvhp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ytxmhtzo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vuyrupvh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cflrxcfz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wpourgqr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fpqziikh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qdyemosh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fuetmbar.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3igqdgqzz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oboxchcz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qdqtfqah.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vwwvtcyc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hofivcfm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dxixpopw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3spdgnsjj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qimkvpwu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ckzgzwfg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bzipsrrq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3eqtovjev.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qkzthihc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jciisbsw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3laaxinak.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dxckyiyy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qlkrzvya.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddhtvhfq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3omzppcuw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3txhfwwcz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nehlcnij.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kbxnagmc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qoljfuhm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbickpuw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3wihvchbc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lscicopq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pxqysloa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wuwphpex.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3utkbgjup.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3noinkggc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3iqflbflv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3abnwwllb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3curuufza.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ompygsdb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uixyybmd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3akifocix.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ujozoltr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hoqcgyib.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oovotthj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkpufgaj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mzobbwuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wahrogjq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rlxdqsdy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3odfrmkju.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zotfpjjd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dijxbmgz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qxisgmvt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3amadijgk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wmxajggd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lxeysggk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfpztich.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ifryxxok.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3etkrtezt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dectdhqt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhujzbwv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lejhjglg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zldxzbmu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vinzticc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mjdypuio.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pdaymjru.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fhccpnwc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xqfnawnz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rdjbutea.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ocilrcwi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dyghepzc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3asavvvmb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hmwbpkci.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jvidkxxf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hhpmnlul.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ukrjgdlz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lsnloojz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbfnssjc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhlgkrko.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoggnfsu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcjcisdl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kwekzgzo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ilwjfzry.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3orlcmjky.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3weetuoyb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rfddwtoj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ivetfcqz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wacjupdm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocrzjzhp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3bxyhsdlv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dyqwakow.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3baselawl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rdqqtkgn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3igxcqawp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ydvpedtb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jkubwnet.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yeagikvz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sjdvmpeq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjtdhho.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3eniruljh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3rzfsmdxb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3widouzom.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wvpfonap.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gtclujrs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jzzlmyzt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bosrpkti.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mlwturld.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3bylvmhkg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kwfrlxzw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3snqgxhnq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nsgoqywv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ydsnpejd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3boddjrns.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dtledahd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3aiexqlpx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gbqxjxgv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3smbypeub.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3frmhvowe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wtnqxpua.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dpxunavb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xwxldbkw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3vgsgcksu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3tnjhzina.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3wyrwfrso.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3nksavsmj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tbvuwese.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hqyqvbtg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3iqlfrnwt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3puopfvcq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rxwoqaxs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3oecodquf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ceiwiwcz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3snrinacc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qvwgqpiv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3wgmntssy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3glkgirhf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mamiflsu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vjuxsgjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iezhoikq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ausumfbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oiryyldf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jmlfnoxo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xkqhvfbu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vkiampif.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ryszpgjy.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gjvkrlxh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3huuvrtwu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3rhenaoud.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zpkfvton.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rzbkqxia.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3egmbrcye.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uddubriv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bkazbztq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3mmhtkxyk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3sjxsxrft.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3dhimhblt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uiejfuos.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ctelxpdn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qlwkiksr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kcouoxdn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hivyckos.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lgwqefkk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3eondovnr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rqhwohah.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cubcekaj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3jvcufddj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ndkgbeph.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3fwaxjvcl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3avstlzzk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3wexzkcol.html


<!-- 参考信息 -->