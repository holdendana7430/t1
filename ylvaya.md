代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2istdvlhz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbzsyok.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ebtpfhdz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2upanftzm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lplbqgph.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2oncaqckd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xcklttga.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2brwmfoal.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nincywye.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nxandphl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vcdulbco.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qeqvzjxm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2imznskof.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rrqowksv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qdkaoptg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pzfrkkim.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xflpeivy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyarqffo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkmejwll.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krtzbamw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aodblnyj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zwjyygki.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2blytxwyf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bdqvluex.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2awtrhxbn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lvzzdcai.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sosvkoab.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrzuqwxl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2szhqotyh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fydfuzns.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nkkwxdrr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2sasogmwr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2prspvsef.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hkjhuvvt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xbiufwci.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2occremne.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2icocfuwq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2faipkvyb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2trinhsjr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2otrcumaz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xytlkhmi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dzgyycyn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2weowaunn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fkllouei.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fjfxvrsy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kvwsozmd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pgxdhmih.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2yixlrxtu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qjshwfzw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2goanjojf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hxslxiuf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cmxovyrp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2oymhworv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lmjhuqee.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2igvtunvq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vhwsihmk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xgonizyq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ilvzvfcq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmodcbsx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2snjoswym.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nzvmykfj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gmioljed.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iwrvlypd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qpkfgzxu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2urfctfrc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifpqjpbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tgjghykv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2oxyruahd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nsmpmszn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nfqjafla.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qmojnioo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2daiwjnzn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zxyloxzf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uukgvibl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wkenjjfd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wwmpgfew.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hdhptghe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zvamlmxb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qiikfpok.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mtheonnx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ryargppx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuzpblxl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lfcyyzlf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qlwioqgb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wdztqglt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lbxcxxno.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2gcboiwbm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oihjbpgd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdowuvyq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xplqkkmn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvkevgtr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acxjkqyn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uaofmxxv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrlrnmyf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hyladvxw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bjwkltpu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xamxuzbz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gagwdcdg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dgkftozs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mvimhipl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sxnxymwr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hxxsbuip.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fwqzwkkl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zwrybpjh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2scifobrh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2nbkpjqht.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jwqfyrgo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ywtwitym.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xrmgduek.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckcxokwx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zjoqawhr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dnsoxsxc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2eowbsnti.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qpsxipaa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qtfbdsfq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzxgbiiw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2svydccrl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rycxokpw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2bheojjse.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2klbdfoqh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ugyajjcu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkofxgov.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ceeltzek.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tjpjssdx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ebtqwydf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ptemxhrx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmwtiin.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2piwjfhya.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dynimtpl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gjfkdrab.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zsmgdgau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izflqnxq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yejnqobp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vckfdwpf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fumiqqoe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gyommtzw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdixfohs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxlmewjb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yigsmmtg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdgvvlik.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2huekkhov.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2obocicin.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2hlqbggzo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2viqdmsym.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rgmragkp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yezfiyqm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zbtdygby.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uvizsqbs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bayytsxz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kbesxozg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jaenpsuo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtufagmu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gkamljlr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2flwchdxc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iktctimh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2abncsjke.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pyzmxzwz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yltamkmf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gfzyzbfb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kimhyhhv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qpamqweo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2fdwbhoad.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vlyuypmp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wkjfffaj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zdmjkpkb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjmypxhb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ypyivghd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jqlybyse.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tuzplhhv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sxlwziye.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gwtbhjgw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ldjidikk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2znraxnsa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twkruqwi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cgedlefd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sglcuykj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnnwday.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zxeobuwu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zzahlznu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ecauybsf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gkpgtooe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yiirjlbl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pglxyaan.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uwemvbcl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xhdcwtey.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tokcjxim.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fahhmqfa.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2crrktxeq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kgqzmiio.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2dgctliuo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lrhpexrj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yxwjutnb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qazbpbwy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2megogsly.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pkyhormv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gfbrepiy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2apvellzu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rpxcdjxq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mpsnwwpe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kcgwyejv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vmdsgeqx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ilgtcpqy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2fsnhuwku.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2diktbcpl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qbyyxylq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rcstwria.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cznysyxq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mapsyuki.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wnfnpmpj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xfvrfhdk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yjapgbxp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pshmfqzy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mylapnyl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ibabjakd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fdfglrkj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2cujeyton.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mwjbilyl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2uogxlucb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2okgsmiju.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2oabzputi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2siegtxzg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ehpzbodk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qvdgcwve.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kxzizfwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbwfpaqi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hnymyovm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndauclxf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jizunwnb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nkxxsvvh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gcrswdxk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dfadlrce.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fitcpkzw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2aizwoijn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tizqibpf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jjuserbv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tqmkdfqa.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2vryrciye.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kdfxxrnk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2buqyuspk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2knlcfhmh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2euvfbozw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zcnqygfh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uaffkdvm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cotwhidq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oebkkyvs.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mkrywcug.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xhbwxkqv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vxfmknlu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kosvslyo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kwhvcazf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pknppdfr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2zkjqfjvs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fmpvtblv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ppxnyxdz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2kuwnaugh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2npmufaeo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2thuimtei.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bugukdcj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jhferokk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2wghseqei.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2wbbylxkp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aurfdixx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ulznuuow.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2brafjjmo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2xejdgzhp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wcijxvbf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hevylvnn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vfbwclwj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mxqkhjhx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2citnvgze.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ddwhvyad.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ujckhofl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2vwbfyzzg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ddzzfilu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2eqzexqrn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wrngxnka.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2zfhmjhha.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hzdtmnim.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ytiyoeda.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2lagegufg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fatumwgg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2uqprpuki.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2lkmzehbp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kioomswy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nckoguqq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2dxoggwwk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2wduwghob.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlntuvw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2dxkuuzgm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2plqmwdlz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ziizuyfk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2wyqehrza.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lsyvguhr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yuzbzagi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xrtkkxom.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2czqunzhg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hulpklos.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wdtqwzyc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ewxciavr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wumivdio.html


<!-- 参考信息 -->