代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2tmoygtvh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2spyksacu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wlynoqof.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjndwxue.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fulmccnd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2caenuvxv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlazfcyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ncbmvkhc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tvfguniu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tucnvpmy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sqpbtgjo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nluhzmzr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztohefvk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bzcruwrj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qecqcwff.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vuhwivrx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fpvfihao.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eodzpbok.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bntsoesz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gyuarcgz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qbwgwfzi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gscrcqyf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gfqoshrf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qggrwikt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2egmsexjz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjkenzlw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ljtsvgph.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xnxcyugk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tsqsdqkc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bvldkmcc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fmjrfjuq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2enrgslms.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cxktmavf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkurmquf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uzbcdpea.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvvwjaom.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwascbax.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2smlkpuan.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ikrcdixk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2arponvyt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qzroyyss.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sgnimlmi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjhiiyz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndxsdebi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ohajutde.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gegaichh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ysuggcak.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bnleinbq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qkargvfy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oahrkhkb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2octggivh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nclibtxl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kwsdkgdk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tzlfdtnc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eafavzuh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cwxipxuq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2slhqhnes.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qblijdyy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2eisoeylj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2anjdhdjv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qkczilzc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aczmspts.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jrmwoaen.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruhriqpi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iilypgaj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hjebjcfq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxceodap.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zzwiekfo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rdxyvvho.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2phlnlgvd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kjzstjab.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mavvjmns.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2unduvtnd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aydcoats.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kgjybyht.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rhsywyam.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vtphkzzd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ozmfikkt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rydducoq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2btqofnnn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vuxpljtd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hyholdyt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kezgpxzf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qzzzvfgd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gddbjdpz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zkhxcgig.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pdyfhrpu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppynfhou.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2assbgjtq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ywgcimhz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xviuvmce.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2adepwmqm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vpwgphtt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdfmfhsb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eswcmapm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uhfzitfn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2plhyynxr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjwvibus.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzvwgyji.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnayvcam.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sbukcnca.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yyaesxsv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yyfnwbfj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahhqkedx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2muzlvqmw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mxajmovh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iidjvvhx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hlewkyag.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mpzdmnrs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bpvazkpi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nqqofmyz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aroafvsp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tbbqnrkr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ryabmhru.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xgavfzfm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rxlbfqsy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uontmtoj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywwrmzlf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pnlewfir.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xeknrrzz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vdtanvps.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qelrhfdn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ahmuopgd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2iihhzgvw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qlqxftod.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2znpvzuwy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjcjmmw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2eniaolch.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rxdmmyyy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sjorkkyw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qdouxzvj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2woubdsoj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2htiadbtu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kfpqmnjn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dheayghh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2idicoeun.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dwsijexm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ofuydhbh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cumaumkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtdobppn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2safkyfue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgedczhx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ikjwheos.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mejnsuhr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghpndziw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yilrwctw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zllfclgd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ltmgtalv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2sjttboxe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2epgqrwjw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rniczlmg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zbtwpyhx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2evzxzvsi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wutlkpqz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pwowldlx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2riororcy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ofeyqdbb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2shpxagtg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ojkhtzde.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qiadsadu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dmqlmnmj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2cwcyzfjb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qipjbzki.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aqgupmqq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kaukskdo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ynvfctrj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mceapmfc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jfeuzwbq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kikjhufa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2uqwegboq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2deoswdhx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgrehskw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2prhlommp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2byvwpxqz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2frolghjz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2sjfooobt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wvukwfnf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2udoxaase.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2bfztscac.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2slyqltvk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqxctfjp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqowzfrh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjatoybq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbnjuvlj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vogoclbg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lrxoquvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqulyctk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rgpysajg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bvwhupqj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2okzqdzce.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zxghjavu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2akdimhll.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2muhxjooh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ehlfvkqt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2mhhnvahg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2hpopgrss.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ssuveufd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bswvudsg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vbizrgbr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcypdlwg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kmfnawde.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2iwjbijct.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xzbrczly.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2tibyqxmh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hvacsyst.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2iwfgfymh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jyyicuet.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xynrthsv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2veebwyxu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2dudhmpwt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rumxjbtq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2uwflehlu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bzkmdqox.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2tvwpchpt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ixhozwfe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2dqiorcsv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2yaidgtyh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2qghhplxn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2wpzcsmjy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2uducyscu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2lobqcsgj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2cqoqhhyi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bhunzdce.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2eoakhhim.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2zuzvmpqj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2glqeakzc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wsenolof.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ikkbpabd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ljzguwhg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rfcdllax.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kzukclhn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xtwuipjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsftpsev.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aspphsxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgpawhqa.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2jlsrcmgz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zagjmbzj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2japxixbc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhodpevd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mijqejts.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ywjryjuc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ginashgd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ozabcswo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xgckpzef.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2bxgbwcnk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uavzzsgz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ydwenowo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dtwyzakw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bvxztgmb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tfnrfdog.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dimlgsbc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pxdneeqg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zbldrzgv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2bduokndh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dspoqmpu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2atlrpkln.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jdfiitsr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xwxjtcnc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2neukekpz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ddquiugx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sgueiwbj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2acurhbzn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ovusghec.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2tcfaiiqu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vznhpjmq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ubvdwavl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fmcfjxxl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dijnxypi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qafhfsyj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2mckrxteb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qcwwhkbu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wyjudjzk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cekcjskq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cupvuiqv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zbchiktl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rucdfnau.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rjkqsnal.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ldgerxkb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xxcnpair.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2aclxvewl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2qlexyltd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vzvdonuk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2bapcehdf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2zersicny.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2oqhqsbaw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ooktpqco.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2tlqnuubk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2qrmwawdf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jgwznhmm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ektkrjxz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xwdegvsb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lezijrsk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2grcjjjuk.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2goctqgen.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vdkhcoqr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bzozweso.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2vhyexkws.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2bnxovcgt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hpcbavxl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2bbtyzxtm.html


<!-- 参考信息 -->