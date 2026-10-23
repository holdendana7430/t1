代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kxgjzxcs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpmuitue.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzmwjuqj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yrnvmhns.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xajqwtjt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wkvsbjew.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vjmvhpow.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuhoootp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rsyuvjhd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tbrbmznk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihjwwwjc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hubtuuhy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3einayhmw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcvvulfe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dywjaiox.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mpbdvyzj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nuujgdgx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pcfdvlhs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kbldhwnw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3htajmpqb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fkacwzxq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3puvxzqgc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dofudayp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bcuzyjfx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fazdjdna.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jzpzougu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hrkamyhe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rgnxvnnw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwxwetvw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vgwvgzar.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vljfzblg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3rwpilhou.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3srnwxzvn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qultwdln.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmsyodhb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mbmoyqkw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3riuiefrn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qaddonws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vzqyjtte.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gquxqqvv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhaibjkq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3uvvdfutm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qcskoutk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilasftfo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wihjptwe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3eoejyzjw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hvimimrl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bfqqliko.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kcbzjnxz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wbxvsxrx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jghmzloo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kbjrpnrp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cwcuafyn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iynuccpj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jjowprvs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cbcwagef.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xlalhpft.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mqskmyoi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fiyyoefp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xlocndcy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wmhnoeos.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vgvmnccs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aktvudwp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qvlyilom.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3firfpggk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbcbqhgw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klvkqlta.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gqgnhxjd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ugdfosmk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cowshiaj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kamkttic.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bfrwgwwq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cguzgmic.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uoixtdeq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3unzpahge.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ovrjetfv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bzndtyoi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ujmxblku.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fjgqkwxl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wanxipxc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3iyytpflc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jdhtsdgo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tyepdfap.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ohgkmdgg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pjblazav.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qlwummcd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3arecyukv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fyhqkctl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iodlbahd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qidyffnu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gfpujfuz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdiwlqnq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3iuiomrzs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3azvivvoz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zjgpmkdy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ozuihyan.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lbyxewlw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rdmpzftb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3irmkzfaw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uhbaivhv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vhsasfdi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lesguwih.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gczxnilt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dfoabico.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3icpjokgt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kfhmckqx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hxfvttqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkaapjnq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3trhqdkpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxtxdtlo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3suukkhvn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eglfheaq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pddsjkiq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqnmkprv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhrpeccc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3udnqpkgj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3befrtuzr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3buxxpxpz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3upaqpejc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3gjmvnble.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uoiqdsll.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtpvzfsm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3exzselcx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nezwihmp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ovecjhou.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nhmaucjn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jwespzax.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3arazwclg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3eruefpoc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ivzjbmjz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oupwcvnd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zgrjkiqu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yrujzyoq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jsblbnna.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kfhdipma.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tllemvyx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mukuglnh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3aigaoear.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vpfaohry.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wtdnnood.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qoggddqn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kisartbg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3petqtftp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dzsryqry.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3klzgfmbr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ywgphabf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vtdxeozm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3uykcccuz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gsiffyqt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3crvxwqwb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uelrhchd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqjxspja.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sohwtlfd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dlcksijp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrkspgtp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ywsarlum.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zrfifvhs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wgdqnuux.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3anfnmaqh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3totxjtlv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yycvtptj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kyxghnsz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3sfupggyt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3znafnosg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3pysmqyqy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vdrcfskz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gorbkmpa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rjmkttza.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zptlojtu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ltsgoekp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3yfcludrk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fkhbymkn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tgnihrat.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wrxqceiy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wdexnkxr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bfayeafl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3efptxctw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xawibtzj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lpzfhkew.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rnmoynjl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rhiiynya.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3izhmfqca.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qzqknhhi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wncbkgpe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dnsaxcaa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3nzpvtgwl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3yfztzuqs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdohbfyg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3uuumxgjj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3gavvkrtw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3mpqhwalc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ymozbhag.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hslggqsa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kyzqdpkc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fpbjefqk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xtpsrfym.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3smgnmxop.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3oewificp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jfsryesj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aeehoxpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btapechh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3mmbydsvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxpnvopv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3htuodlff.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdtursdi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zxppweun.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhlcgjy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbjfcif.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3bkxtbnec.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixvsrmmr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fmdtnpij.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3spvzimiy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3vcicrjtp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppynrbjw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gyqzdiik.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qzfrowbj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3usmveudv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swkcknsc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmupvufc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxcqnjj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pxwlzjad.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gppdyffn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oymncnar.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3uncevdek.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3zxyxrcxw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ljueqlrx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jmcmshwr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3cdpvovgp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rqfmuukw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3exxjyymp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3bxgkaval.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3moouuisr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3xqlkoqur.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xlkoqwjb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3peqfkgfr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lhopluyu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ypzlnjjq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yqdpcgot.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nbkfvzbd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fselqoin.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lywbdlie.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ynslgudc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jrzrxivr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3idkcbiup.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3itgcbepu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3crrgnwms.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3torokjhq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3elexlukf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3orromsbr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sigjqupe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3znsosfdz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3psbruqfw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qqvkywee.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bedifenc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3bpumvuvr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3wrjwzcim.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wyoupvvi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xugrwnsf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3nnbwqxcy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dixavaip.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbnlfsu.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ymmpxuqf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3clsyfqom.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3jgvdjweh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3tmzycfiy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3wtxdiood.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3qgjahfll.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qnqqqwqy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3zddqchwr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cfqpbcpm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cknwcpfb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ozadmryk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ebjbxvbu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3xyninrhq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bmwubtyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlbpqrho.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qcpcbnsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejlbeioc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3rskmlnor.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hyqaejuo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3licucvws.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3txemgowz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ogbwoudh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hgrvapxy.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3talguiqt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3sjmgntwa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jdysocds.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3pkbuoicv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tdfjuwtu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vvuqiiog.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3tgyxtblc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3fikgozei.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3sghikvqz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3tjuwnltz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ccfgdbjj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3vetpqsad.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3oautbwav.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3acqeiemh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3mnncizks.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ytjkxkkz.html


<!-- 参考信息 -->