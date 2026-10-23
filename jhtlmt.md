代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qcdepnle.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jobucigy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iaydydnz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3efqqkpbv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xhdhrmst.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3sqzcolke.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3erhyjolw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3advfwcho.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlmqsltg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vjapclrv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3fiaqjogi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqxpnzvk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mihdufvv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qhexoazv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3agdxdecf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mbbsdfvk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hbrdkqgo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kmvtyduv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ewexbrqk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3malnvoip.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fohtaeke.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3iyiyfjjz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3yzrnpvnq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3onvjylrc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yjitocmd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fttfdbmf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ytexiqvn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hcgldqrd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3izhuspvk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3opftakit.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fkdoqywh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kquccnmv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3brxvrwaq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jellurwn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3scbbgprc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuyytuyl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xhjvztfe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bksqhmms.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jlehnrmt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3einwdcep.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dhbqbljo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vstzayse.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uxaccqdb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jaxrlmot.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3glvjkyis.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nalttvfc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pnllbkqn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dfxyznum.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zcggbghw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jixdcecm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ezufyssr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlzqqewo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogkwshem.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kndnpnps.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvytvach.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gpylxlbp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3krfwrnsi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fwkdiziq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3sofvbxmo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iayucdlu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gznxtmrf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwlzfspn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kghmfxed.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pbqcpbcw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mhwdtmlw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kydjpxsx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xcvjqgqd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ynixozaq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uvvtwmrc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ufkfqzmr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kzvnprxm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ovbkdmmd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vcsbadvd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3omwedzgz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xticjmot.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3trdxefen.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ccgvlktw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ujamfkyj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ztgxpxim.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ofsjfcxj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jmqvzsjc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gecffzyz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lifrydnm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hneivyyh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gxpginul.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3scemuykz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghwwrdxa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvpxjdmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ltfxnckb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rkvjuuux.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3obkpyrab.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3femnursm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3emgttweo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mitnygjc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bstgdwgz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xudekcih.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xgtjxefb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jasdvwdi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tipdqvii.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gbndyihy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kxqgwsno.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3agdvytxh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3prdokupl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqrghreo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mzlbsnwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwcutbxl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vyrlomhg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zpjqtzne.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drzghmsa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vrepzack.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqvclpta.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iizsvmpr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gamiwuit.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpwkptja.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rsreaukz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jbwidziu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nvxuchla.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdfkmbeu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bhyxnztm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pmsnasop.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmllxzhk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gkihlbrn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pnjogind.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iangzqhm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ibxzfjpm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3exaeecat.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3onlaqtwn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wzgqpiaw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bnabivua.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dlljsamu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmimzmp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3nmecfgit.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wowygbkd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3axpwbpbg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tebpimuk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ergwncdn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qskzmysq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3figdimhb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dlmfmzek.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3bpuxmlpf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gtwdjyml.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytzoktde.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ulnywmzu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3frunimkd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3lqhdfwla.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaciorys.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvjszzty.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3inlsrdgx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fkcqkpav.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3scihqjzl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkczcuzv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kresvfns.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wjlvfguz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qokboooa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3efiatkxk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yqelwpvb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xkufbjhc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xvzqwpit.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xhhegbbi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3luaczsqb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hvwsssbb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3aelokxhu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wzvswfsa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xewarcgi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ajbbqzub.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zwoqqmsv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3muvryxok.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zqakcusv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3clqkvfbp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3iovjbgdd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3knkxlvyr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ycwfcfmh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3kdzqfkjt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3hjhkkoow.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ojgephqv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3rbyzqvag.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3iocajsue.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ipbwsyag.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yzaxgdxh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3uxvrfgqe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fpmefrpk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3pggceanf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3eusyower.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3hxoyifya.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qmjedjkd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhdzunj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3gecuzdfq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dynmphkx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gofvqeoq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3zlsrwkxd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dtqfbpxy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ttnywjqq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3khwjazta.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jlzijgkn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ohuusupc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mqlekxbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abubxhzd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sdirozky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpecdrop.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3tswlxcci.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3plgsctdi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qjkxbjsl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxfarcnx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljsmvkbj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pgqygfgu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xzqyvbet.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pgszbvqv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xuavazrh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3dfckxakb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggkaumtt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lfizxnfy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3oiosuale.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qpgauiea.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ntnnsyfn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zipnejvr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcoptbs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sokztjcj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3uoaboqql.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xijxqtsw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3mbreivbp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3guqwzutr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3wloiunlx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3sholziki.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3jcircnmm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3avhdcmre.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3oybwynbl.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vplhiupq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ifbdomdk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3swxcaept.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zkmqqydw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lmqhbpty.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nofiaoat.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3uycrhjiw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tahrcwcs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3koicgqpv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3aqfbeejq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdvlnucs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3upimefrf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cpjjpnlx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3clbayfsi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3qaqjzpny.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcjjkcfr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3geveludt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xldzcfin.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ifmimoyn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kxhjpryp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ifefchsy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cygijpnx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aarkzxqb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3aaosabia.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3netajtxv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hiivrvld.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lzuimzai.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3svnfgong.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3tsqmqjzg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xnkdwedt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3xdkhovas.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jgacvsds.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3qysvlxui.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rpyweefu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ttppphui.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtsgwqj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3toattbsx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rmtnlxaa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ycoiuhyj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zaoyhzlk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3eginqshv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3posvacsp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3zjuatcmg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3cbxvijdu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3leetiewp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjljicrf.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3fzqxcabp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhblmuxq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jfgspnmr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3qftszpwn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wqydlncj.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xofxypzo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ozeapocm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3twzrsncx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3hgwvdtfo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3otfjvkev.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3wkjxfjml.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gvvwkbtr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3scxwmxdm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cnioylll.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3mrhzsmeu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cflhkfql.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3yxbvozxn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3hikxvtty.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tyiisaba.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3eawlitkm.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3swfysybr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3hdurxkfc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3rliyqpqw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ibrogxgc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dajovevm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nwkjtdar.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lprenovo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ugkxdoti.html


<!-- 参考信息 -->