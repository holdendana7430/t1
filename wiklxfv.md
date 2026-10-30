代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gckomzhrq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcozwcujc.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gwonkzkvq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghjefymwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjazmotcr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzsltxjyy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnhkxjiqy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gioigxmyl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gvngtugcu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gduuonnbx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gqirfuuqc.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gxanbjzhh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gtgetsueu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gioewcgja.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/griwdkvzu.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gqyuauqza.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/glawwdjre.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/ggqdheuoo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gsrzsmsxx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gwnqfzzmk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkjxvjaso.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/grdneevri.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqtjzqbac.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gwuioxhhg.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/ghfyvjwrp.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gactabzzi.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gsvphwtcl.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gykcdoulo.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gzcypbeja.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gnrddzprn.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/ghdciupvj.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gtgkransp.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gmmuxdgng.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/giridmzsd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gusmxfntk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gedftjfdt.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gvnbxrvmz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grnkkbuzv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gcetkrdvp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gfukgwbze.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gbjcbqnpy.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/girziqtth.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gahbmavss.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gbgvsqwoj.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gvlrowggz.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gurbtgoho.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gbathxjcf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gjdsigscy.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gfyevnmjy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gurcltjbq.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/grwfwlgku.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gauuxevmv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gfyymywop.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjchcgxqb.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gyvvicwpq.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqwjvtuin.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvmrlvngo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gblillnls.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gkacuixjo.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/givjavejw.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gfitphmbt.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghxjhahqd.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtgeqwsau.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfqatsdti.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gduqyfhpx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gqcjrsrdx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gxhtplbds.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gsecxhrsw.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gafjcffzq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gcdimueyt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwycidrnj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ggazdjojq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuqtixek.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpbkzdpkd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gafjdsaqw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gmlmecube.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gqvlinkdb.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gbolanrki.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gwhmubdwc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvubzwmtd.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/goituczqe.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/ghzwyqrtk.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gawkoapcp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/ghqxszkol.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxmxwbt.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gjevaqsvy.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gpmvfwkpk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/ghzgfvbas.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gkvucstyi.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gnrbjqhhy.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gbqdpwcqy.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gtwvwvtlx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gkvihiudn.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/guspiieto.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gaersvlou.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gdfhudalf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gprmkkkvw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gcrmgkmbf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gkgsqhhkm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gnlaeyqyt.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gnmpafbsr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gcukusqha.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/giwavvjjp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjljvvuej.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/grwccxcma.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gjjfqyqqd.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gddlahyvc.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/goijxsbzh.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gfphesbxu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gibuvvayn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/grgfvxhcg.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gofnrhazd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gcjjcpxzk.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gkiqgteus.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gvggpbwrb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grjbeqgbi.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gxxapyjns.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/guuomlxbr.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghzjjxyle.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gqvpvuhmh.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gqslunpsk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gsvonrwan.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gizedrenx.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ghlhwxpkc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/giijlrujt.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqkgwzncf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gztbdiajp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gdnpfwhgx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gvdqifjfi.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gzrykkjnr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gbtagfsby.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gatuwijtp.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gkjzjoblk.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gdugnkklj.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gzaiuftop.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gsonjvils.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/guligdqtk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gixhcbkxn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gianndpps.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/glypmbssc.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gblzwbnwn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gygjoguud.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gnyjtfnvh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gtczwrtbs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gcpvkdstg.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/geulvvwyx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gswnojyit.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/glanakhpf.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gmadudcbx.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gxwcvqyio.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gclcacowo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gygptjcgi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gqbqpauhy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/govdvlyck.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gcwbixfok.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gwrhoelqq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gvkoaqbdg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdkrizbyl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/glivoench.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gfjpplgnn.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gfpvsucez.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/grffqzjjx.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/grsxouomq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gywuwseox.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gpxwnkvtx.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gxckyszdw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gupkerwaj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjmwnzzwt.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gdyszflmx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gawwyxvww.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gkmsqhfqh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/guupwrtmf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gijgrocwx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghyscwwvr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ghwyfkrhp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gevrokwhq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gxitjpclv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gzrpfmfhd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gqjguxcwh.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gxnczinng.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gjddelmph.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grpimzxzb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqcjsjgrv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwqzovpln.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gfnvbbepz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gsskrizeu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/guhuzxacz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gcosfvvzi.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gyzggcqqt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gdkymrhbg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/giadmnofd.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gagiepoqn.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/glxfpbjxi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gkaftzecg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gikgxgvbc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gfkjosdmq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ghnryxdjg.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gikbjenwm.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gvfgxmjat.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gunovedgt.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gtagodzqh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gasnrfaau.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gdnjcfdoz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gqantokgo.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/ggebzehry.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gycosgmoz.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gepervoms.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gbgmkudiu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gqhmrqaex.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/ghspducru.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gisfdmrql.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gvezmyvxn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gstvgniwb.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gtzickaur.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/grbfsuwmg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gocqghalj.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gnxsiqhpr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gorxcprkd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gnuitsnim.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/grgunquao.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gxzcmomnf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gystqkmja.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gabjvqzix.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gkyaxcsls.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gzuoexefy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gtozsmzzp.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gglohvcod.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/graexjjpt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gmoludkgv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gmdaobnuq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gfrshoyis.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/grealtknq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gdqjlhmdm.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gngiwvkun.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gxzpzklzs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gtuznbrrp.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/glrwyvrum.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gkjblvxrw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gsncoippk.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/golakphvn.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gmhwfetpn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/grjipelro.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gckthaver.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gsuaivkld.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gyvjghnhi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gptpfqaxv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gdsvmequt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gtugewerp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gaaetnbku.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/glkwkduju.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/ghsldakaj.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfvkymi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gizakpeeo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gksegwvhl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gtcwjcoio.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gjcwgkdck.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gbvhaykgr.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/glhxzsxdj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gjjzecjpo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxxyprdcq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gowsktqxj.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gfeyqncmn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqxzixkmc.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/goebmdtcj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gbzirhdmu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gpuphirkj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzjhgynjm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjcyqyede.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gkxspocbj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/grvqhcpzu.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/geqcwnlye.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gkycjqhdg.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gapgojonx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gscwqkyjm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/ggghbyniu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gxhxrsihy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/grpayivdj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gzshxqgqy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/ggaasvrxb.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/glihjkult.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gpcuhmtuy.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gjoamejca.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gpjfqsybt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gutvberrf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gziyqanmg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gayjlykkc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/geaduehic.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gjeukcwet.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gmvvpdxno.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gzmthnzwq.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gpjaqorqm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/ggtavyxha.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gqxzpyuud.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/geqxhaycb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gluijqwkr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gfqapcyaa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gotfhvclp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gfxsbqynj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gvblmakbv.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gdgsvypcx.sHtML


<!-- 参考信息 -->