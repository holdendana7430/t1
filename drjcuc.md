代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fuqydaib.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmdvuzyf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nyhytmyi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bpvgmflx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pwgdwxeo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2khpmhzda.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2usxafcgs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ttdirqpy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nigpkgpv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnehapem.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uicmesrr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2itgmzkce.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rkkwnrvj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2kcdeztiq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2miwelsbs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2skythgqg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fbrhwmla.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wzqzoxdn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqgqjvtp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rvdtsomv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dvqqsyel.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uhfhvbis.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fiqubmdw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjktcvkp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hiekyock.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yktobqmx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nlkvowhj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2frfsbqeg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2txciknqy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aunmluig.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nwxzbpvs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2youmhzgx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2igoaedml.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xmmhhxdy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2esxcmkqh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bkcjftzr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gdpyvoqb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2thfahgwn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yxvatzqt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2geihaxmw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2twiwgfti.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pvakvcvi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lihikcbm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hksfwjcl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hetokeds.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdaubxmw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zreiwquc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtjpswza.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xzkxdgij.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vpwlosmq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xojbyxbt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fvfypiie.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zgcovqzs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2unxdzeam.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cuaxlimq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2etqpdhus.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gsniqney.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tfwxigpz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xqvjcpxm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gbxfjzti.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tzpmwwsk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lgjauqlt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qixutmfj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fecaskqs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zqioghbl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2usoucghx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vgvhinck.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2slkwixzo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lswknfxd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiklhujm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2udhzlbso.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tumaythc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwtlbkio.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ridwgwpa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vugsxekp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2confiddj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ymmqgqxo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yasvsvbx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oaemwvlu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fifgtvrv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xgswyvmc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lwapfuoz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bsagqexy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mfrogetx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yzmbxeib.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nwjrkfxc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vwtnylwl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ynysqhft.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kwruofsy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jqywleum.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dqyhlcbk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jjfvvqdg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wbrvvfbn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ptagxmmq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qxetgzel.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mhbgrsbb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ffnvghjq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jcbjiild.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uegyzhzd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rujzmnoh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bpinevwy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jjzxygpe.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cnspuzcc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2somvwssr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2edvqmlkt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yczhzffn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vhlofvvu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jelwcmqi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2oqhqpere.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aajorcde.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zyjsbqon.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ozsgslsz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qtxuzumk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xgjrjhfo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2btfetmbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdjbvuij.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ghrvehms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jalmggxz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pbzwujnt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2jpodvhzd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfqaqzcw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffrsgjwc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zkczwhdy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2umdhqrnk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bonedyjl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vkcxhqxi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ptdawout.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ktjyxuwd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mxhhotyk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2khokcvum.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlocccq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zspxwskm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddngizyz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zpcitcyq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pajvnwmp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xjsosbno.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2djcfliob.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2inmglolo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ibnjjceg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wqbudsml.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dvmkixzg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bdxrodyu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cpwtblmr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2smfstely.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xvsprhxk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnjgqhfc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ftrijlle.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bnbbgxie.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mvyncbsw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cobarpru.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvvoisyf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2tdeiothz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2twpxtxlj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uvjdjtxe.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lmthqbta.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2plxiacrb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fxjnyugq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcrmobup.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mqasjktp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2dfhcwgzl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dzeztnxy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2thxtoddt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mugpuujm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ntqavvfi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jdxckkmo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rmhruksx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qikbfddk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2adlrtzyy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkgfotu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jryamrws.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrboajo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gtdtdlmk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2leivtuon.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2skhuymky.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yxiwiimq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zfsqvmod.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vegtswjq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2kklwnqzh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wsmwfner.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kbadmixi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iimhgomx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kooxzfje.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lhxvqeyc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qnhwkamg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bnksjwup.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tntsgnus.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2dqoygztg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2acvryvtn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mghynald.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yjyiwfzs.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xvtojvjs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lnqcxonp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2pbrmcsyt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xkwmqnpa.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2txjieuro.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2dxyysevk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sclxsgzx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2pkjeittp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nvpqnpkg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2eydsarsn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qtupxfgi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2gldoggmk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ldlpbhxy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wzdmwwju.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2qtztouuq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bxqbaarj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ylemxcce.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzeefmaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jylafclk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qovjghbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqpgnxjv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vadtsvqa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xllystye.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ykrbrcup.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfphfney.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ckouuyvm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vgxhgmgk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dccnldpx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2doomhrqx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aoaxfvwv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dqvybhhx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbaidft.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2qyjkpjcn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2uiamzncq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2blwmfzub.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfqcsfww.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nqqswqam.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dyojolwi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fdecwbdt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2jxlualzt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efkpndlv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mdufdodz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ghjcidvg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nmclcpaw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kuaplrwc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2htigjeeg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2avjeaelm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vhgvjkcl.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mmqlcsnh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlgcssjr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pxacpvfn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eodqhrqh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bnrsvuof.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zqtoxmkr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2agbqoqlr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kjhixwst.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jsothcox.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jkxojkov.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcijtvrs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgsycule.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xaeipldu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vxusxciz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lkumhnrh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlaxzbbq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uuzfacsf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jovgqnfd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gletcleg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2txccpiks.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ifnallwg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qibuwhen.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2oaaxtzkd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nwcegnrx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ivuxxxqx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2jzjnrbxf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vuyogbex.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ghvtljgb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2unbigzmy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xyddrrdp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tefyvswh.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vzopeihp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2jfxtdmso.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2jvryeocq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2eqeqwamr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2rcmvskcb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2fstekqaa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2oeuaozqx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wxrfvhac.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ftvphgks.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwlajxx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rhwmkojk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hdbhtkda.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2mzcngesi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xkkouwpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hirbrcyi.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2bnpezsti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bssvroux.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2arijcwwg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2puefdwmp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2dpqtzkmk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kfwficec.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vmljnzix.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2yajfcxrz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2chpnzfgm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2oitpgzdf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2coujgqgb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ohspaqha.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2febocqdw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pabptjbl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2swcxkhye.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2loghjixv.html


<!-- 参考信息 -->