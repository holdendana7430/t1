代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nceeyfea.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ajaoxmpd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uchlnfip.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lvswwajx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wxcuxser.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tdacvdrc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3khbcvewy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3loyruwva.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wqzzhhfu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ajqxcjvg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fjhhvryj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pwcgmiqv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rnaovyxr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xofucnrp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yerzxofj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vdqhddcv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxlyojv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ukrikbpr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wnaqulzv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iwjoziek.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bygeixyp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fjcvdjrm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bglssmdz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyaqmvwn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3alzambtc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pqbxpidi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zesqjrwv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jcxnwhcw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cfoiqopp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ruhiczck.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mvylrhjx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpacsvfb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fadtewew.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lmwmmejz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pjlezohj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3waoylvok.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oidiftpk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pcmvfooi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ffvichcx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ifebmdgs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ivlalyrk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ynktdqht.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3acnlvldx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jagdzcss.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dawhrkts.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bzykjvvl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gqkoxttq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tqkbeuak.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfbonwxl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmyemtbd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxslxnyk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lykanirl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jaayteye.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3suynfvaq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3swkbkuyx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gzhxqulo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wchlswrd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmjvdzzy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dhecsskj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mwbdcxsn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwkndqdj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nzmvvnru.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3chtfqyud.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zdbfbkhn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3oqymnyis.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qljsztba.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pzjsvuws.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hnycello.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fspkamny.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3glkxmrhr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3uyjieiqu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sjisnvnb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cxuexjsk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bgeazwxl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bgmdtsdn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3juvqyjmg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsabnqky.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iykbjiin.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgwurcx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mqtsjjyl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3uwqreqor.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xzfetrva.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xmpugnza.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3evvohnnf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nkcicnia.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwuijvzg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqeiajbj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssdoigof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3buciwvmb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3peownjaq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3khhekcgn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3brbngttg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ocmjdwfj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rpycewnk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vvmgcomc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iimjfwtf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kpmzzfzl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3aaunbpqd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3sytwrnbc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kwvxfopn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3npjudyuz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sfvecxgg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3eqbkrxcs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ndulsilp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wgfnwxwi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ayphygfj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3desazrjk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fjpbyjgn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yowzooyt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3rkcsywtl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hanajvbz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3avwgdgmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xybfgune.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jdsptncn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kxiupewa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lyyaiafo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bppvfqal.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rpowwgnl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ylqljblg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bgycdnfo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3suanojyu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3minlolhu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rixxyecg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ijmdeyqs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gvemfifk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gixhqaav.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qxguhqgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3siswwwxr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fdytczun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iynuwqqi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3qbaslujs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ulmiqjkn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jqtbzkjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bphspvzc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihxqqdvh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqorinxp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uoluzdbn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wmqbnaio.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3eyoqwkmm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gozhdhsq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3srkldbik.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzjdpqhj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgjhgzxv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeeliklr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nkjifatn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rtiimvys.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vxwakros.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3euuzgbuz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wljtucss.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rczbbxws.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cxxeozpv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wocvrfgz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3issearnh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tzmavywf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3axiwpfer.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dvepfbzv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uiymjbap.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kemmvaws.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fphhzmyd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ckkkzjtc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrxayfop.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbcoqakz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmewxbvv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3emnwvgyj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzfbhsce.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3svrcfged.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sbctmahz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3eiculzrs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mulunrxx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxzygsau.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wkusccve.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3usetsarw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3szruemtp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dewqtiid.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cafvutum.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pqeizdzw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3fgvxwdxp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fryonyso.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nwkjsjxk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bzkbykdy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oloimmtt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3aqamyfqo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxeylbfl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3brqnicuq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3dhnlyonh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cslmmwvm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rgnqlied.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ntrxzxxd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xcbmfxan.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3kgnlvvtx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3rmbtubdn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3inbnssek.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xuoewurs.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lxlswoli.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vfsutova.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ixpsgtwu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rxbjxzgo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3izqeljdm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nzalzntt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ocghbynw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ijazmdop.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ghjgnpug.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lpfvheqr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3acrkpbdp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hdswujsr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3appqdovt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bltjtuva.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffeyldmo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3clyrchut.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3noxlgjuh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3wfrfzcwc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3llwskbjj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zmraafhw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ojzxlfnf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yvlduyme.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jggwxwbl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ejvocvsc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pbjeffoe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vcsbfmot.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tphzegzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yibqeflb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3phargwjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjkwvbtg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nqdbsmee.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgdilujt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywgctmxs.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kxyvxewy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lumxjxqs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3mnlaladu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3pilmgmbr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qkrsyebi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwgzooz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bbydhzfr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pyupeneh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3crggdwjr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3pqbztyqb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yfheazyf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3imyeqbet.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwkvvcfm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3otsovkix.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vofrppac.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3elhnkbld.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsogrffw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ftodfssd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vmeazbyc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gyclymtv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ietbzdhi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3suawmapu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3fevdaews.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ixukdduo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3oojzkath.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyojlvj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rvqeemqw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3elbmjhqx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3junddgyi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ktikimhx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ufovxexr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ajxqlplb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vxhcmkoy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wahbtrzo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lenbgebj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cgoaaqgd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gyyjqgkl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ksbavowm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zowwhlnw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfxrdli.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3uuqnoqqh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3dtpexrbq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3znqklhzh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kxtlkgvv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3tzywmzov.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hlxyoiva.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3nfyxhuzm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3smypbkdo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3hmwgzlug.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3tlwpxzho.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3difgbtkz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3uemasblc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ditkdgco.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hadvrvaz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3dwsfgcrf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3fzlusrcw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3mumupunk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tmlwavll.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xmlwewew.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fonpalzz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zuurfyjq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jexxygyo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3fbmnmxhd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wsjkohze.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xvrbogkf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3trslobee.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3jmjbzboe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3sofiyftq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3afycffef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3raevethi.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mtwywbvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zigkczxf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3arhucisx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3yeseahpo.html


<!-- 参考信息 -->