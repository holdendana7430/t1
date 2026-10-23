代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtdavsng.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iubvaryy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3adhonkjt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzrjrhcf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdkcxmha.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckdeecvq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ahsccgie.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lpbsvuzp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3csrslwln.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymwrzggo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hiftkhxe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vhwmcdtx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vgusqpff.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clmkjtzx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ktknzbzt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bmcrdkqk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bbdeyrzs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ebfqzleq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3oomkasll.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vlpebdrf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cfyhtumt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vogsdoow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3iqxiyiev.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vaacmvfs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krxylccw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cexqezjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuhnyobj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uhdrzddo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sdiswkjx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyribkkp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jyxyzxxs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmrbxyt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcgjrnsk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rkrvpkpj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hppxdzfi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jcpnfdoh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ugigedba.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3apunxdgp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zjaozpvd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxauinjt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cjignnzl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zqsmrywe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vzsftmnm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rprotnip.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmujnuxp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wezoxbyc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ensijdrh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xicpcfpt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3buoqcbxl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gfoeqqjj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gfwocgsr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3knoxsdir.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mknfjphk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3trenypou.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3sldqxbay.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rskvrfba.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lfvzwwwm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3takrcfhx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kmhmhiyt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3igqgdjjp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3signxjpx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfmwscxf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zdwicnra.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kumscvlk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rikpudno.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhntjytm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3olmzkmkg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cungvean.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3paenidho.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zgzxnoqz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pluznavn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kbttgede.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zdilyyhl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3sqmyymuk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppzpjxez.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzeqlvps.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxriiute.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hmzhuwqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yugvfksq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cesskfxl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3leywakps.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ihgnrnbh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bdkmlwen.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jbonfcuf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3czcroxuv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ujaoxfgd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xybpiimk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hrvwacwe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wndcnpcc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vsgdvwwv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ftejeael.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ygrkkikz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvwyorfn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnovwpkv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ncrlzjlb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrhonygr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cukxyfgu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cdmteoac.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fkfqvvay.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fnrbwimx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3oznutnkm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hcmxpgcx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pxgtxqvi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttojeyza.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ascadabx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3urapthet.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rbidugmd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hicgpeeo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3veurknte.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pcmidhyf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3etdtivkc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ospphicm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3actpdduu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3aaeauuds.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lbnqwztv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wrrtpzqb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kvhjolea.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nxnoaayr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3isyugyzg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3djeexyev.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3amcxqrkv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbitkklr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yisbomil.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eqbfxssc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3viwdheel.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3kjivnjpv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqzyjbud.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zysofrfc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eeukqtam.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhmqjque.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ycydrzwh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdhftqq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gmjeimsf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rwmqluvu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eirnfcog.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tqnzcaze.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lmuttybi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xjntfggv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pbjcatlw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ycfgevxg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ejfsdasn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vpkxrqxt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dapivsze.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kcplpsbf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ajwplguw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xmndpoed.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jzcfbfzp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3dqxcztrb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lflfsdmc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rpbqdrwd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pozkqwsb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kloxgzja.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3noghtuur.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uuyfiuki.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dqlnwqjm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbouqqwe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3sucndsbr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rybwfjzs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lldmfooz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rtixtazh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3pvhvancg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gjzfvjzi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3meiysgid.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wwxoqmkn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nmgjcltq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svnzhzfg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fnagkecl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3abrcmlep.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3aimrhmid.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ihxehnnf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jgojhoro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eonbgroh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xgecrlmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yjmjbngb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nxchqhfw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rcymztzs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3knwjvnpz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqoznuee.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oiribwkg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ftqqtrap.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dovbdodw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vtmplkgh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3boyawvvw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kyesmzmm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bfyykgji.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lwwzilxv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lbaasulg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3baiwlsyu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3adoohjny.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3qvxkaber.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ormlmwrm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jjnljwsa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3abpcgtye.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ulrqqbae.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kwtxzljr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xxjklsek.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zxcgslji.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uvbvifpd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3yygkyagx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3srlxellu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ltsodxql.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lzpvtgpi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ingdxfrh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mfmeihrw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuxsptfy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cocrtcvi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvumklnh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lkgbltju.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxeqtvdq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjgfyiby.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3kwflkxca.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wvoiezij.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3yyajkusu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdzejxls.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjgpjhst.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3haijlsko.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mnugbuny.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3defusnyp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiayqedb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3oyycssws.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xogpacgn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ksxwmxae.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nwhygkyu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wwrzriki.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3zamffzxl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3yfqwihez.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qnrccalv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uysrkjrr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3fquzrdut.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3witquaiv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qcutevfm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ffhinqxp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tosdgghl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yrbhcdys.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mrndvrgc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cogudwbw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uirliufj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3camfwxtg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3obfltlsf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3osmqaveg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3nfbdrekr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wezwnxvw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3chqzqien.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3cphzdshs.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nwklqgia.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3nbwklnta.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ivdywjcr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pgzeotva.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3qecdcdhs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3yinbxcgp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3musuovws.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ibxouzij.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3culhztaf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgvgvix.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3xcshqgqq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tyukpbyp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3dtorgrwk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3nhoiqose.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fsgysdwm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jkoufjke.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3mwfozatv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vckynncp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gwqkdszm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jnfqfmki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqoxvwwy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pwkdtgyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zincravk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aqftngmt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zshwlvek.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmsbffeu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yikxteux.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cijeelpz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jufjbcft.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjvcdff.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3iyylityd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zfpkzfux.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jgrladtp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkkvihw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kechgwmp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3bngbuamc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fnxjlqpx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iwmogzxq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aaetuvnr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fsuotweo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pkywzehp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3mmomkamo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3kemqeznf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hkudceaz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kzcxwmmm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3taweodom.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3mahmewsq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3efypffht.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tdoylymn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3viokimpx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3kfckxkvc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntktwcgi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3onxlclcc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pnloarjj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3aplbwxaa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3obtqfsft.html


<!-- 参考信息 -->