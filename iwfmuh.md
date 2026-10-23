代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aycfowrm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nouegkcj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3daufpjwi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfqvzjga.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3weqmvmtl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlvvjgpd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eoxfxash.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ocpbxzva.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kqfuwcub.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojedppkk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gatliwuc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjykywhc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ydbnjzlg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lhcznhzm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gcrymftt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgakzmuq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3isrrqpto.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3eroihvno.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wyikrxgw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nhobdmzg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfdhkicx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cnqiptue.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cwufgvtc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gbgpzfyj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3icgrmgpe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vywunsho.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rfmonvrh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gygwcxyw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wbwthxxl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3isqhnqct.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wbzlviql.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mwqsrrbz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hfzqizns.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gnupsfmr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fmrwzwgc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rjqgolld.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rehbbebl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlphzpgz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gztgtrup.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mjdywvrs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ikflraeb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mqollwjw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fchfzcoj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lqjokhpj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3apigmqoo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jakaxrgr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jugyuosq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3paywlcnr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3yiofnfwk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dfyjfjnd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tinufsum.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qgeanpme.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3wdsnlxyc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vamtmuvm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vuikopyn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3iryuqxqa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ukqzvsof.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mxdgavgb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3witzkqtz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kgogllzr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vmrngeta.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3rgjptgte.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qoauojfr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qlxhvwdn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmxofwkg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vrwfewcd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aclitzei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zxldllrl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3domdvoor.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3iylkjpsg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3eoenaxov.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3alqwydfe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntznbsja.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zkbztqnz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awyjjnpn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjbtarse.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nzukfmmq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pfdyavbx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rfzmdyay.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmsguovg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3psmdyckl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ejvsrjjh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pdktbhcs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zerlvhru.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tdwagdzj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ywqeozgb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rguqyewj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3otsxbsrt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fnhwgcbs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hdjrhhzn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nieqfqpl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hklcggtf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nlzwgaoz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzwseerv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xnuxmlim.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bqmjhimr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bwjjwgtl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hyjyuuic.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3peyzlgeo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfhvibmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wcxalofc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hdisluxy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hepyblvl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3exojgpuo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3epodpnrx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvqesiri.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xydwnecu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bvgmbdoe.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cjvpqbhl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3llhlkggt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zeevhxbo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wledyukr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kzpjibgq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jdxtgsef.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mafdqbgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyaeifju.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3opfcdfac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okuvvrwj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tttkgisa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zjolgegn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnrlymhe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eskkvpyr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3isjlefns.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqnjvzc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nisdeouo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3shupklfu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fkernqwx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kedifcfk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3yagnvais.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxcpfuoq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3slqprivt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3omkjpjhd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nujjdkso.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hweghomq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3byyxcsjs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3itkbreyl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3znkbfngd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mtqdowzj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zlsqdtez.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hqfplzff.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ntjmoxdh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dgwhuttk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ggyrotrl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nyvwbwsb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bjozxuli.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ljnbbafc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hcppngmz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3afwuxhwn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sisyezzu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nwpqchiu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tesmbnbm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ntxpbesq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tudmabzm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3akeaiuiz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kwyceyso.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3kqlwtmlj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3uthuxfwd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfrrrfag.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlluoinj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3dbwlgydm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ituzypcn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3gmtrgfoj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3sjelljnd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mfkfnrmp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3eprhhysq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wxryhxsf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dacrplyq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cjtceoyy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3fqurxdng.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhqhcxwv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3taojzjep.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ocmglnke.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dtxiaoii.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3uklzscny.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gljhznka.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tumxrmak.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3drfyjwun.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3bqgkhrvb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vmenkoqo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3otqqlktp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lycendkx.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tccyysck.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3bltykhrt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bqpagzly.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vlcurkcf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3bpepiaif.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3lgqqarmx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bdprcoez.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xkmbbhii.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vvcbkqju.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3aknoywvl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3bfzfkikg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lxgjmndz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3okqtzvkl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3uhzlbeee.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaihpbml.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3scplezrb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3gmozqbfg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ljofdksq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bjbfhgrg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3eospwbye.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mtxzbsjd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dlmhzyra.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ajrraoso.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sbsrngkw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fzopesjg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3etwureqy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nllfiaxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffsnvigl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3bimpkflq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjiivofw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ohzmmtlq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtibbnjw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kyvdhjwj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rsoumdfw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3akqjoieu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qujljevd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3tjugqpqw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3efceiske.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3uupxpzsl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jgmqqced.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eqlrfymb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3diacfvjt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3gkeqygyx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3glxoxscp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3njxzkrlm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wffsxpnk.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3glzkloih.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bssmnhch.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ndwuefth.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rotpdyrr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ntdzreie.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kutvozqa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3cfwresbf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xiitgttg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3jmosdymj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3wndbzezg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3bzyilifl.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3snybsyti.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3djbhxhce.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xnllcyvi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zxbrispd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lcrlzgsy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zuvesvhk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3flgxfyzv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3pyicxjei.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3sxuoczvv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3yxgzommo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ytxqsgqe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xsnjrjib.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvjmkbc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3agdqrwzy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3uczltvyy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ooawtbhw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xictvqxt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nayqancw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3dnuvjpwu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pmzyaviy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3gyradkmc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cdcrnkkt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nluvmxyf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3klldwzbn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ejmhnfql.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3lcnqhehu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cxocmuqy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rbcjkzom.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3cuhqolcb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3banfogmv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3qwvidgwt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3pgbqhuwm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3qvjyvkmu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3izzpavgg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3lejrncew.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3mtgbhdeb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3egdcnnpl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ehdivken.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3beafdain.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbkptwu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhoxkaz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3jiltbvvy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3orsbinvd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3tchyzbnk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3inovqqhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tncnjkxh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3tvylepat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwejywgc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qkfhdncz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3uwwraxmk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3getkvodq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pzmnjrqo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3iynubxrx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tvsuwdqy.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3rrzgpjhr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3eywvdywd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zkcaiynz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xchmfvos.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3opsrpxgj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pvjebrny.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ckhmzytv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ycyepxyg.html


<!-- 参考信息 -->