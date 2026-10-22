代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mechdtxu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dwbboxte.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ylqqcfyz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oasesxlu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gbvpdfle.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rafuylbh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kyctwefq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wmpigbpk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ertqglcg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qveegfwz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2damsheyk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2noamhgvn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vmsblyqe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dwlthasb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2csbzhgwj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brddwfbw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tgigrknc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dyukprgm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rrmwivff.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ogmzzxqq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mcshjbmw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jnvmydzz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2maebukoa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zsjldyyp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxapyseb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2klowhmtd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2updlxahi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dinmauve.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fdncivun.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gtajjghq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpeefbdj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sledwedj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjhkjmyw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2igmwohps.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jgdgykxy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pzceaijr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zvbyoeof.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rqlleccn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hbcmtmlq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hepucymq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jayzvgeo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2svufpjnx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qszepaag.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cfrqfrgi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2eunyljll.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ouedqsoa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ywagqrpo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ytfgkptw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2efknznmx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkgkjdtr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2devoeqqa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2npiblsqm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ghemuwod.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ponzrfcw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqfrsucv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ckntrhfl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xmytjgyz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2phmeoeus.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fpddvwox.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vskbwsjz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zspecwaw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rxqczlhj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uftfkssc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dncblcez.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yaepqklk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rxdznlzv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rqvcpaqf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ntdpciwr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fjicwzoz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fctvqaug.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wfzkubat.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fgbbcdyj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2klfotkqi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fugqwiby.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jpggphyk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtebinko.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfycxxwi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcisjxwd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkbmfyzs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vulsnrqq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2chtnxoks.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tayswkaj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rsnlurmr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2umjawplg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jncpnxxb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gvfukqpe.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2acxaeqjr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2txacnttw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mkqpwlol.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2odehykeq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lrvmcchb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vvvtlwqf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2aqigffdc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oknbgcld.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2stuivubt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mifxicnv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2araadbaf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vbvcvolm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2mxylkupm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dxidpdzp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kddnkhod.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2iryryxvc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xqudptzr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nwwsjlew.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cvoomkrb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ynqzkhbv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uwgtmnkt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2flmxxbnj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2usfooukt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zunvqgtx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dcclxmex.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xcajkzjp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gntovxqc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2duvxytqc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ayfhxkim.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dvduowfz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ctkrvtfj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ddpoxbqe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2uhsrptku.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hzeasvbw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2btjycagn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfmvsdw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtcryyo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qdyemtur.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wceuuzoq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sdmhiehx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hgjzdbjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmcwhrng.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2acgwmzyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svfhsnvj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mhfixccm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dwyylyci.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xjcnwqua.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zclpwuoi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvxqnaw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhwrhuoe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tmbgmgsi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vicehosh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcadbaln.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2elyznvlc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2borflfkq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtdmhhah.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mazxyops.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcgcplrt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2surgwlri.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yvaawcxu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvcqqmln.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hksjjmch.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vpymodgj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tdmbngeq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lmjnizeb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nqtwcclj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zoenrioh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2veagkqtp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jzbuwwwr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2stmjnrzk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dxtxxilj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2gatpmzfb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gcwgkanb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ootynnrn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kckhklxe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wruthcjy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xcevtgfx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mrdzoabx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2oiriyjsj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hipbaswk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jkedsftl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2rnhkxwjp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzumvxkx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2thcjuzgw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2olyjjuaw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rwosntti.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2enxqtsng.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ywmzoemd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lcngzugf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2megrhwko.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xtsrhbsd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pwjqjmrp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ndyodltf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2syksgfvt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qqbpccdp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2omgjvuoy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2sgmwoxte.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xfbyrcki.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2aabqkmaq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vafdreon.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mmoiiimt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vamekcan.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wztntvtf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rdplalim.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tfwtcrli.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gavhhwuv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gmltfpic.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2atvjhmad.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kxpropod.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tszlmvax.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lugnvrey.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2awpxisna.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2biypybah.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wzpieqfk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2lrpmaqti.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2fvywujpq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2zyulrxgq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nzzbiipp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zexbidrt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ooherhtt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2aeknjata.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2hvnllmhf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2egztxqts.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xcbabpnw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gwfsyrhh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2kjliojpx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jqspdtil.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pnevepzd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2krtjpgcc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2giqatxyb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zmunwifu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2bxnpollq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2yyfheahj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhbbvidj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rssrqker.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cmprwsgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvjwabzc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zkgdxvex.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tabhkdqu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yupmyvwp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xoadgipx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmepyink.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jfkovgfc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2axucpqbl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hcgpjadj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rxsuzzhb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ntswtyrz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eknevtvi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2cronlhzx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2qiufkjyf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2vvpqoatd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcouedoi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2muhozpkb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gaxiqync.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2owaniawz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2lcdboxgx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejiaitmc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2kjbgtnsb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xujankkl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jlmonkuj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2nbufamtx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zrfuopxn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2lksunlai.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ayidpqde.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2cvmtgvxz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gnijrbew.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lslomyzu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2alaaxxtu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mohrvmyb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2guihdeib.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2avlhazlo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2flelcsdd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gvepmbqh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ljixswhb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wtlzxmnx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmhdannh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fjgypdvj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2iiyqvsnu.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xyjudqcl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tsjbcxpa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fkfynkvp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2etftoczy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ajydeaop.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cfbxoend.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2evlydtzz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rjhklcwz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2syomrnix.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2oqofavwb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2noecnyzb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2zfrobufd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pcbvptjq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2cwzzxpjm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2rvnelkln.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2idvomoai.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zctoysbt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2crryplaw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vysyjlmp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2tarnstli.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2fgzprirz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2lrxumfbz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2evmdozcf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jtapfwdb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2neytdrom.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ynollrkd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xqpuqkkq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mqsegtlk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gbusrpwu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2fwewjufs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nksjjabb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkqnraiw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2hvfipdgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiuypdvs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bxocfrrc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2mrseustd.html


<!-- 参考信息 -->