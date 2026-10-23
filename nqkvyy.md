代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yvnypynm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3coejfqko.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yfpkvhaj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pgroquzj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhkchvkt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmhdwade.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsosvtdi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rpmkmidf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rjrhbghy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xzsqnfzm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cgbgipnn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ymfnywsy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3edyvbtir.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uzknfwgk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dthlfjil.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kjwyqbhn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3winbpytz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zjdvwdie.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ieaenbnj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qfwwiqqo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hdgktwpn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wsonfxpw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zmecbifg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cumtvbjs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnwivopr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ivomxlki.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ugzikmhk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pxzdhdde.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3avjlhvpu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dwbhsnoa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3focaretv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3txdytdhx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ftfqzaan.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ahipgvzx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pslavvip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pynhadiv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uvpfnjst.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oqqvotag.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hcuklpnr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ahbqywwb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzcndsjg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fnqiethz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmbkcxcn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3usrjujng.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nhhaqody.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3krmsvrph.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3igquunmy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dygertzk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xszwaiag.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxknrlor.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnexzl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qcmzhxhl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnpjnnxi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxrgmqc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3oplgshoi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdqggrkk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3deaxcchl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3aenniyqw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eyktxrgj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fyuozcwc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rqyttklp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hetnpvhm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vsgeuqgm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bgcxwebg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3abamvrgn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hqgkgtiy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3auytndgn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rdugdluk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3syflbues.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhpsicvi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmtqzmrp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3igsaronr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tpehybum.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymwyunfi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3reuwsymp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rtfbklgi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aqhoocfn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kknhbubn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fcbxvvaw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ebaevjlu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dwktsgml.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3onaitcqt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uhiwrovp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mzmumeay.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tqwovhvu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3orleqpus.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wdjulnqo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fangwqod.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vxwidnai.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zejuczhn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3chgoiasr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fonpkaix.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vijqiykg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zenqhlgo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3igjocpkr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zacmamke.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bevkixfz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbainlfh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ogglhngp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3szkuqdam.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvhqskw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xnbtczxr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jkkedavs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufigtakr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ihgsqewp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3axxeglav.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gzgajhdh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3spqdnmof.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tpfafmuz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xktvptda.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dqlnfbms.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mhqumbfm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cixmlcal.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ocntjogh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwvsdmtm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cjwukany.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rjbqzvpm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ortjexxv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bzddgnnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bveiffzn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xwdesmdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvfasggx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nslvdidv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qqcitnty.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3waumxohi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3llaxfbas.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lehqqvvx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3bwrdnakm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3igahhlhs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gbgvktke.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uvgfohhj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fppghhyg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3waoxkdnb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hxcmzgwt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cmvniyvm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3buzucike.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qzqndqpu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ljawpoyx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tjfvzsxu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhqowci.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vpyzorws.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cdscqhpt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ecuxuwqe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pttguvam.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wrabdyoe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gwwegfoq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3oczxarji.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rvunegkb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tbdmcpoh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lpkwbvdl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3vxnytbbc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bztrigpg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hesueawh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3annpmdlh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsizgxxq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ssjarjli.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fyldrnwe.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3huwpogeo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zpbnfdbm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3pxdhtzhq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohkafqaa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bnoiawml.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpddqayp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqonaumt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ptbsxivy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xdltorat.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uciniyjc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zqkpgduj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3cvyozyom.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kserjdkf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jtnqfsty.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vhwrpzpm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3paeieyfc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jchifano.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ebufdwig.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3exdkpatr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3arlobdzu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xsviieuw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ovwyjyps.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ypwjmozx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gkmtqlpt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3norgqgjd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3bmrphojf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3axqaaxxi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ecgxcmjf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kfmsqulm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gxpjqqvb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cejbyxmf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3uqttwjbm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3sbrlffqp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bqoeggvp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3vgfaaigg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3rncmlhdh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3nhnnoihu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3tljdgxof.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3alqcytit.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3lrzqnqnr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3uiixpomx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmohotb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3magfeknq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zxpiibnz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3duofbblv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3msbncypn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dcnrdaam.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ixlpmyqx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lcjebqzw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3aottfiig.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uvueiszf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3acetzimt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tmvcpcvl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3oahwrwgj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wqksonkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdfkterx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vocwxolu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aygfgusc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3erfafhfe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jfarmfcu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qkwbzjhs.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrlrgbm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwklcasa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rdelyiof.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3chhtueoo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqldvzpf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ufpeeeop.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gyyetsec.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lankwfjy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jlqqlgji.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3rflufcbj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3uyitpvzg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gymzdhue.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwbupzg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pmpbidfx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cjnwlvew.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ebzcqbxj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjdyzcig.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qertvzlq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ltviewxq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3azldsang.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jpqvuqrr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3yinibiwy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iwqskhno.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hvbzsgtw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vjgnyhed.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ullnxgmz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qxtthyku.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dgbyxlia.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hfqazued.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ywaxlxtp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3oymovpwx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xwqnhpjp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3onlchuds.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3cwpepivm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3edsrinry.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubcxwpga.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3awecsebc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jupywfzp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3zmttdeuq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pjbgyziz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3eunpjnfm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3eaootpgi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3btbluono.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bvkadtjz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3eygzbmsr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3bfviyipd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rymnirfj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tuhqrupq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3gijnoqnn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3mrqeewyv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gicxcxum.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3qrnqnmbk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3zctdwypw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aegvgpir.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ynmanvxw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3kvfoavpd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3oocnxmbu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3porlwzfq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3urhhziiw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3sofxyzpf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3khgenlir.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xjtcgyex.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3idifcjwp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxieauk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nudmuicl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ieiuadld.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3nbktalpb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3uwfoinhj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kkphbrby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exmuyvju.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gmkkaqvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmkucdci.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3uaxztmym.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3jgglbeqo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kdegyjsp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zqtljdyw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bxuhyfup.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3cpygmdip.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3fmqmporv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3exznjuqf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3sdusgtti.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lcdhsetu.html


<!-- 参考信息 -->