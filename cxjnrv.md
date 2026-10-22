代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbdfyeie.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmljqueh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zagmzzts.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nubracvc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnpvhdub.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hjwmfdkj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2prmfywot.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jsreibrj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dewkvkik.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pclxrykf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2duamuqbq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rdaudwmk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2grfowjmb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qqvbtxbt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wmbmuonw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xoswkhis.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xydabvge.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2riiyriso.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nufvtxrb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ykdxszcc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fyhgwqab.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcbvlfdj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rvoruvdg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hjdveogq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kqqyznyc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhojpron.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fyxterni.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kevkiqju.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atgezxnp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2cbtngjhh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yudpgcfl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pmksjyqc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lpufunky.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jhiiitpk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kasajsap.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2inmqvyhc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylncftrv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gmmfpihz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nsophefz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wiwxhmkk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2elmbyuiy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dsskgufv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wrvmwrwv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mbgtniwk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tgvylbwn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vlkqsbgd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2czuefoqs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nonhcaoe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xvwxhtwv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jomdizcl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zktgcken.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2nlfrqtaq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wvwqzwde.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2abzmbwux.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zkdylyaq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2aytfzgaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qfmawhka.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kevkabfz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dyaosatu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dvhxedtb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sdtzeikv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kogjlchc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tilwllhy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcgiwjee.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qttipxfa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wlfoidjw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ycenykxe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zawfgbrw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fsiduyvm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vezdfhwv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mfwbzfih.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nujyfydd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2keyppbre.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2etgrpypv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2npmtxvis.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qydvtyhg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lgpegrqz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2masbztlk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xvlmgznd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2coijzrlb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhstyyjh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnvoovjt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkhwwefe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rgwztbkt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gimdkxkg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnhtusra.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2uffhlbor.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jvzpfsrk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2okguntbk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lagohkvl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jfyggwxx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2loyezjku.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xzzjtnxf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uinyhemk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vgzxzohy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dxjmtggm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nvuzdkzi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ivlsumhj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hqdpwrrh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gmsmuxkf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2axqoxfpp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rsatbjiu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gwvnjxgx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ziizewgx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ihnlqohs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ibswbpvz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ssdadstu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qoquhdph.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2egnsbmvp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufiqlgjp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ekjfeeut.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nlpedbyd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2yuzgplke.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2lrywsarn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2bmgvokjk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hucqozrk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gcwqpsqy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xjkiputp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2buitxlqh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ryoubnyh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2aqzvcrbk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mpfahlek.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2pspsgjsj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cwsrecww.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2deibbqpz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvvwuyqk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rjffsjaq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2cfttrwvp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wqjvvzro.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yeorgcqw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gpwjdjur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfqatqto.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jxyiqrhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lppsiend.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jhfelxju.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cziejjho.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypnezfkk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2skktnljo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ftljofdn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qcytkzyo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2aunirzmk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcbtmhln.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sskgunsq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yqssvcim.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2szqbxwto.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lldhhvgt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2savvxbgk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zidgtgis.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drmhisxb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qbimmosy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tvrpixhp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tzqyaamx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2utprvbrb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sgkbbbby.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2satnjemj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2njanegqj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yfxhpyhi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mujdqcuq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gyblagks.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ovivuyil.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fkxfztca.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpnlhyyy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2xgqgjuit.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nffnfdob.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzkbmdzv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jldzcwey.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhovtxza.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gdjiksts.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzmlhfom.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ekoxtydc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2grhmauqw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qxixxrdu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jingjfln.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2umurgbyi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xbnixjxp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shkfyxty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2emudbwlf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qyrjwhsz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2pkwwigti.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uvuqundy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fqqkwtch.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gzbzbann.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ypdibbqj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2brcbjvyb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2amvponcn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tqkkvdhn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dyyzznjt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rvltopdy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2fdpxeklz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qkilisyt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lcyrsvmx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bjaykbod.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wrfyycyf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cdhwxieb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2nabhoccw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gtyfjnuo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lhljmlar.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jjkzptdq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2shsbtsuf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qebomwhc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2uziqrqcd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yeqwrsyq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dnthkvxv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wwyfulph.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hmvjpueh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2olrrvlcf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hhbvhrjj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vexurtlj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bqrqydfv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qdyuqmqt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qwuyudun.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2xjsxwylf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2gitqpnrc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2kcyeewoz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qbllpmks.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2oamuxpqt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2cqzvvhju.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pyhgkqes.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zimdlrck.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2spbpacgb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ezctgdee.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tiskrhvq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fwakqdxi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sbtdowvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2biusncws.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wwcttfgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbelnjlz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cntscukq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vhutxqes.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zbjekjng.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egylnfpr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zzdiqcnj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lbzijeoj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2cgxsaoss.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2barilabe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bltwvxel.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vvlzlaef.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2feoipteu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ruusjyvu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vvjntjqw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bofvnjgx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxclherv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xshwcdtz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qtnpeboi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2txzcoxiy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2rgnhjonc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qauqkhfu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jtihlpsl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2rpxpjcny.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2qyhaflmk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ohasulqu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ytvijdwq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2znvomzdi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2zchircmg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mpbprhbj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bktoqcbw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vuzxbiuv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2pzbawloo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ovvcqjap.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pzsfzdpp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gmcsbuyh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2iovyhcsh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uejwrhni.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uwiefrzr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2tslkloyy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hdudcavv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qwumzkip.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mobvcuel.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jxooxpfe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2egtvahgv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2veuuxakm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wlsxvydb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2znupcglj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2iydmsikb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2jmkhtvvg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2yktezkyn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2rqsexqfr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2oztfwtbu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xcivxyke.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2psglrrjv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uocypxxw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ujmscnkl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2fnableqk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lkdolubq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2azqetxle.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ehbttlma.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2tufclwea.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2pfzuomfw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2tlrhymxl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ohkwumvu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ujcluchp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2icidvyqq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hvhbjynk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2brjwzlzv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2csebelme.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nhfmtrhd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2qpmgldxm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dgbuqwhz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2motpobfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smietuqq.html


<!-- 参考信息 -->