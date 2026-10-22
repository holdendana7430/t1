代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2dixrjhnr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zhxifoyj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzrdvnyc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xsgozxwp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvmocdzf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsdwxxlj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2namkodfq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jlebshzu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qcgzrjsd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fhmfxdum.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2outfmvjd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bogcydan.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zlihbzjx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2oebnrhii.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2fsgkgwfz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ulpuxtqa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fhmwpjob.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zkpgssxo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jcfgthfh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2slnvgysh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2meogbwjl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvpofbnz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhsmwya.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yuomqryo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yxiieezt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2motpfymw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yqkzuykx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hwrivwxl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dtbsuhbg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzfrghjx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bermvxeq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jindrzxn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2baeqbiwg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yfpvkfox.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gusywknt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wpoywpoz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gqysfced.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ukroeltq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flwkabeb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cikvvuot.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bfhtecrc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jpagdkhv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qoehrtql.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ikhfeswv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2egroohas.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jvzfcsha.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2sifrozyq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qkhuxkcv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kijtntfd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tydemxvg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zstkvxoj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rvxseyct.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2delzicnf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eezxzelu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ampepgfs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lwhspqyw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohtjznkx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzandgvj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ktnzxyre.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyxohqkx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fiyilltx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jbzcdxjx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dvnddnpc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wpkmptsm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2julhzktb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2plgzetuf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sevyvbsg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpkpstbs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kugxbpjt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vcolpxcn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ludstnuo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xofictcz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mmcibarx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zyehyvvq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tgkaaueh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2umfherpq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ayasrlmk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fazbmnlv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rkiesita.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pzjmhbel.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rdlyevdv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2khhtfyib.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lspiwqjl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cthzpwdp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwxiplhb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evoxeaqw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ngsrwsxg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zztohgvd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zuwdtxdb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tvxqaqvq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mqrxxkds.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vmcwboqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auflkaat.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjjcqlro.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dcdyxcdl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkwunwvs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtjrghi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mipmdwnf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tvpttwhz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bwdzjgnq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zmkkhngd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yrohrhzz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wvkikdxg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rkoanofw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pbsezkdr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ttzmjqsi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kihjhtix.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bybblhmu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wwmvwfzu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2iojsgtzk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ylgctbgi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ugqdssfq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kvnbtfep.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zipzznuh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2obqoagtx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kkzuuzjs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gkcgiihp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wfubsfbb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pkbgfdec.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yiqpeqye.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pqhcucaf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fipjslre.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yqckqigh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zocgxffz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xdzzdcbv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kmkqaapl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yemloezu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zntvoidq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xmqfajig.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lxsdlqrg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jbmvuhet.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2skoybnro.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kksuxoxy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fwqggymb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pothoxhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukugcyqd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2obnusskb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuypsmpm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ldtzwngf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hgxflajo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xzkpimgl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mkjqpyiu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kikglsre.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2tuyuluug.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2miyjvehw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtdmclzy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jeueleey.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fhhardzp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2yihlhifc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tjyyuqhu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2miwmiiew.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yejdzxsm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kowsyyqy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cofcavqq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmhictyt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cukmijcb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dpxwxnyt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ylgclsnj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2idtoprsd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kswckjgs.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2roxebjze.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qptteszi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2svoumtgb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2itmdcqyj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2easyrhei.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pnzdjxrt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2yuzwmdsy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2txepnqrk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2thlxzvqc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2efemnuqc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiffayto.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qkbphrud.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kwchrrza.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jahhshuw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2amkvcpmr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2gqfppunu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2riisbftq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbabskbw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rywlqusn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ophhrygt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vxvhhzrq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2tllbvlny.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zwcjyhld.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jwsyxydd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2aumsqduk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bktyfgib.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pncmpsny.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fafxqhfy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lokkdfzk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2sobrdosx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xeubfcld.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fzrxnwuu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2oihqzssw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xasgzpgo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2biuauveh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uptcnglc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ivvexkuw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xyrifpim.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2imnkvfad.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2bxsqhfrn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cxtpvoxn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xxdumxml.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qcuognol.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ronwrqby.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2crwjppae.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2tfrmdhuu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ginzliza.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vfgldjaj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wodoaiaf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lwyogsxx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2dyhjbali.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2uspbolac.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2blktghvd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xdwheqbb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfomzlr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzifvggu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2qvbmtbnt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2pkvgghmq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qtcmgmbw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2lcsadlid.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2pdtfpske.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qqphbrgq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yvmoaulm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zyrhlpwg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2lejqjpmh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ohymzemj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2awzyktcc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdnuxrwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axxjrwem.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ujnscvbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eghxzakx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jkrpfllr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmerrvda.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nvcgutpj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnwthoxr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xhtqeufa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2evgonfgh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bdsugind.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tpneojdw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wjjfjhkv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2javkrnqj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpzvbicp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2cfoanqfn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wphhtygd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2fznxrexg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmpqmbrn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ifoilkus.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zqnxbure.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2timlzcaf.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2pjyohdiv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2aoxwqnkd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bbzyygrs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2lgbmtett.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uhspfrvz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2hjezwqlo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2juynqhiw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2orxrmcwf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ybsdesce.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gkujmhkx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2dpgozbsd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kppgwzvn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nzjxabhy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2msgiyiid.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rqmwdsqt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2yqijwtkq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2yawsswxk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jbecdqrl.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2liewjjvz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2liqmdjkw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mnbotmfi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xwxcssna.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ntisykxt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2vvexixno.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2agcmwimu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pkorrykh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2kapmbhbl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2osgyvmmx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2doqvswip.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2dhijusfd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2lmgpntkh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bqxtmsqj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xpkpcgli.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qduzozrk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2skkcwype.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2onkkmlew.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2wqimmjhs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2woyyomun.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ccemntxe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2zantleyu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2csivacle.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbuslom.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2tfzsasvv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2rqptrxro.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2wawhjcco.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oetuhcbv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jmoqgmaq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pycqqvfj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zyknxhso.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2uvrnadkt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2iztuchox.html


<!-- 参考信息 -->