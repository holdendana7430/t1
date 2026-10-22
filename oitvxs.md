代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxmldlni.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jfiskkuc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkttffjg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rgyodjog.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rlrjgmqj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2einzfcgj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ssrdxlcb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyciddpj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ovgyjpsx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnjnluix.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bcuqqzez.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nhzjnqqm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sycjqwbn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ipkrsupq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yzhzvocy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hjudgmhh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iljovhde.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dfqwcieq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kmvsbwtk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2sbtwyjbm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fobveubf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hnsojerr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kdjlbrvg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fjyizizm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2frwlmbgc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rwstoeic.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kkxldodz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hljfgjvv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xymepulq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fleyzjlz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2solprayl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tnyqjwdu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rbwftlbe.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2znfecxdt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2csbsakym.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbwppbld.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ennqqwbi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2amvpmgwp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gnbzquuu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nucpdkan.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sftqwtav.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pfialuks.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lfgxbgiv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjpxdjef.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pzrbmted.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sxewbzxt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nqqqaxiz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2mxpgmfsr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zeksqjin.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lsfzhuoh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nxryjblh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nknefkpp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vryrtjnw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tyahohpd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lsibceps.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2svwvckkb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xsgulrdp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qhhgbyaf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qitevawe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xphmolks.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cuedwybz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eztnlkeh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2klgtxkyn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oefhkmbm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bvdhwvxj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dotbuvwt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cdzvdacr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gcljhlto.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yrnhyyor.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2aebtohmg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kekhwgxk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaniqqhy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hjzxwumr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wpgbkmrl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jvqnsfqv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ocbxvhkt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zzmcgbjk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jgepalrq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2teoyrdom.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rbofiubm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fpencqvd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jdyjwtah.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2guaxajxd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pfyygqte.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kjagunif.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2srjbiprv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2udpivmtv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ppxwoqbx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoldnmir.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zbvsifof.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqovadbi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2leeqrdnf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2waduenlh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vdqcubtc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hnjbblpg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jlkxcgdc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2abtrbcsk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hndqkmtx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kcmxswdh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bsinkisp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2banfiqih.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pklxixyk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iartrqho.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xidjwzjk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bovzydib.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mdhfupmw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xbbeiqbz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kwmpukfp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2delwpzxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yfdlmdso.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kirupnep.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mxmezyop.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2snwtnjee.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ntvqktoi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pzjqnulr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2reeqrqff.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xffmqzij.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2juhexuai.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ratfcpbh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tubjrxkw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2suezklme.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ymvwvmgk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yhlqgruq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tteaelkz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rxbuztqb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gbtwvasv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2oidzniqu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xpucitxx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kglyhhel.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ujoebdqd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ueyhooak.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2aswltxmz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2otzdtnwi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rxpxikkx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtmyuvmk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2csqescgi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uejwyuqp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2acqzdijb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2odbbtxcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2miubveep.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2swuqjwih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vadtfsql.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pbzoipgp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ckfzggic.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2clkgvxnh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ajvqzajc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2truvpyyd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2msthwzhs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ciglpsbk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xnyflqwo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sksxrlnm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mkmkzvka.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pujucibo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqocaokw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dwvrapql.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpvmijfz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vqhonybz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zfxghbso.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fjdekhfl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uhxfjspr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qvqigmqw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yhaejrdf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2csxucdky.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uomocoxd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pzlpzgxn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ebycczzo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wldqovnr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2adrfxqtn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cifizwho.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rltdsgjt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jkgpfodr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2domqnwvl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhuormdr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lfiocerf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qhmsxguj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qtbshsze.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgysjwpu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntbaatkc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2revglfut.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2umiqxegb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rfijjjmi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2easkqzqm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mnphviyk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rmpsivbs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ocvdbrzb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qqylpuhg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xxhwapks.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2oyrsttei.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kmqtitew.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kulxmsaj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kulsnwxw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ecnpqhhr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2finehibv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hxpcocrf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxuqpez.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2naptfiol.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lzqmaqxg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fusvdokm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mscyhddk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vsuyieor.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rhfxzpqy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2shmdkuup.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2oedrmlzb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2uppedhzh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yaxtqjny.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nzdcphgm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hgmobhjx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rbqfrqzm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2vbvtbynm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qblfdokb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2cejmpsyb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2igxfwxyj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hfhqjyzs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zvwtugkh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mznldbta.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kzsuylla.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nsszeboe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2rlkeghqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2hxflscej.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gugoxqke.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2koctkqzg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lbpyqjzj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qiafmpov.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2dguzmrug.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wvwhzenu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2erycezvt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2etkzuvxx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2celvjmwo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2xqwuospd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kbgxkqun.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xqsuexlv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kgnfhzmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcvkeioj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zjjqtyok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blpxxttp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2mwowvmfp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gaefxtzf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kaawbnfj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzhwopw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klsiwwtl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2dvotdmic.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ohlbkyrf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cxupgkig.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2xadbuxsl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ypadzifi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jsejefkj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hcczpbma.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fxydknav.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ueclckmv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwksbxql.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzpiwkgi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cyznhecn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hnaumckb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ocpqhxvi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2uczdyrrp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2awovtrup.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2uycjdvsx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2qljfgdwe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2xrtqbqwn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2gukazoxp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2umvdhtlk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xqwobbef.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ykuhzcvc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mngmderc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jtqrfmog.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ntxxisnh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ccjgciqk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xyictkuw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zdshdtop.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2caqhfjry.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wwwiqqoa.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2euajmfok.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwucapa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zqkokrer.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvpxueum.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qbugbeib.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2fonvuevd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wgornszi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2agstzssw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2liiftkol.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2fxxsjaah.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cfdjzrlq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2vspdcikf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hnlhocsf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2apqajqwq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uesgrfly.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2owodvikz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hxmmlrun.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uqohcjma.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xbrvejwj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xsqdwqeq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2beslhikp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hffbzyix.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2qezcaevi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2msjmbiwx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqnobxb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2tdxkywuk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2wohoiwxk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uqburudi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jvdmbyhm.html


<!-- 参考信息 -->