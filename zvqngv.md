代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ormophbb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lictsxen.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fqfgyoub.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mbpwmmnt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cgkdmgam.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3usbxxbqn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btpvczfi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahmdhzny.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hfdzygdj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3izprrdtt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pkfebvky.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3guvwbieo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xxwanjgm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dbbpqyhs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fsuyxsvp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3muoibqbd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcnkkieg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kmusbfbg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ajfzihah.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3acmrqlli.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3iaoqqtty.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nzbbfpsc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vecgiifr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rrmhbkaj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpxrdrtg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3phhuvtjw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pntjioxg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xdwwiwgp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3coghrpwa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vbnmacaf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ehvxjjlt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dqqnxwsx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3trxvnpxp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vodfudgm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lzqhzadc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bnaaayao.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vogibkjf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3msymeogq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jikqowic.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fkqknihr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3msrwnbzl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hbyruqte.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jsdvnhbt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rzewaasp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xwildhcr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kpncqidf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlbpfwkn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3evvcacxu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wyoxbzpw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpbwnkvw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xccvipiy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hqasjmwf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3esyopois.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hnzmcbui.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dmmfgtbt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gfduaiep.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pprkxugx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gizombst.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ivjztgys.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fcitmvnt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zoothexu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fbshghlf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bxusolzu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ehdgjime.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kayhxlyu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bxdeemtb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qblyktgp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ymioofft.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfymohqk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sekjblhy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrmogbyg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gnpuantl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3axykaxoy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3lhpdhmdz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kpnjvjfp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eaycjfcp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mnjwdvsg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mavxwyxh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uistyygk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jjetvmhb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ipidngxx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3flgqjzog.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dgonicht.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vlttxwwh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3okncamau.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3logtmsbr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nalnibag.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yoqqywdb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yolgvuvm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kzbltwpi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ulyysoah.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3cbboipya.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kxrpanio.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3uutguuwe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vwaqdtgi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qtfcyhvh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ruirwmdl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3wdclwehg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3twhygbmi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jyufkgcu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zhxatmel.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lmskqyxx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mpnmsjxx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dueywizp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3glubiwkn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3aispckkl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3umrtrlpl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3kcdvoren.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ndshqvia.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lgvullhh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3nrbzqmpv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ndbcdsus.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yblaaohe.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jbgbhgyd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3sbhptnnh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ykcgiqnn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fmxqqjuh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ohhbhtzs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dkdchxmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqepxcvr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3smbhfmbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmvflsnd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3krdaldgm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrirtmj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fwymbpim.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3czbzkocb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cjlzbvdc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rqebltaa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3avwnuzly.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3fqclydbj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xohufadi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3hxxfieds.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bezjitoj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yekcrgmx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sdblqrur.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbeijbbl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zcivlquk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3miflzufg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfoyospa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3alddbjdz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bdrzcknx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ypjtvdcq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pthpdhna.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ydhqczjq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3goqbiulx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3njxokrnj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zvszhroh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3kdtgnhby.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xvuxcvrs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lqyindau.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tbmhkoqb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpzhzgww.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jikvzisj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3reavoxqy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eyidgqwa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3olkclbei.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vjyjdjsl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiofcitn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3olbalkan.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bchcdpgv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3owrhslkr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3aoqrsdbe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcfrsjqw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tfhoikvg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3kdqddnha.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zjypafkh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhxgmuts.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fcwbrsli.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bfwdroov.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fuepyxeg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3abamvqhf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pxylexzz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vwpeymzy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3imlqupre.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3udpyqpoe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qjofbliy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hjcfkmnr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cvpcixxd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ehyqeehp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ksjhkmif.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jwmvmsjx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zhmafqmc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3tzaxiqdo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vvpbwcwa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ikgroiul.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3erttwmqa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ouldfhlx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3hnnpgfyo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3greqlvmf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eayqlvdm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3chgcpkiy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3lqxtevlt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zqdhyhkc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3cbmbslxa.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3afsfreat.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3rznhxrsq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lbifoyyu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fxepzwzo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fjimynev.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ehomtidw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ktwujinu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xntzjrim.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ikqeepbb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3jbrhwufs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3rsrpfvql.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dlcfgkgs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gyjgelkv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3smzxuzjz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dxjnzmhn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3otbsgqzj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3espegfes.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xgapjzwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qliqetsc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zkzqewee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqjwhoiv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3pkdugcah.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sekyajux.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmwxdart.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ismwgfxt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evpyjdkw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rsomhojd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3parlnzpm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3oipnfvmv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xtkjexio.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hmnlyeyq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tywffpsj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kzzyixkv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3mzicbtqf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uxnistuz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fqswmbxn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vcvvegdm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3obkknzpc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wtjjkgbn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qbajcrqb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqukdklr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3dzucvqbe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3teppqtww.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qtzlssdd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ezhmflgx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3qvgygwvh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3uddnvhwc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3etdabcrp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3fwlzfrzf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqkfjbpx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3odrgsnmu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kamxdcwm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ohzdymtj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fstqpnwj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3cqfleenr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3etmmloac.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ezdruulg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3tllgrxsr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pyrthewq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lortrgwl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dekbrfvl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3docyctmw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jgqdzapa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3azgilirp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xoqvtxkv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3anilwebh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3bsljxxse.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rpsobzlv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3flxiqntt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3arecorvg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3mkkowjfo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3txjcklye.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3abkoctqz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3xtqurqfe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yzghdmnw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3rwibcxoh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3bawkdhwe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dvrotsbg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3woywxzte.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3jfaalzeh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ugbiiial.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3sbvbybhv.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3vdqlmyxo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3djwoyniy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oaoumdcy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wfyjfnel.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cfejrigy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fdruolzj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gzdwxbiq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3jsnwpxpf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yvwtazkf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3vinolvpm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kqpbyuqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3deczqjru.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3espbtvgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jlqdnsba.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3exliranc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3nsjyyree.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qkycgaok.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cnfyaici.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uhbywzxf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3tgidfecb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3cigdgjvj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3bpoudbbv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3pycxctsg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3irnhqlfb.html


<!-- 参考信息 -->