代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3luuvscqk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rgctlgbt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbwhmqnm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwzpepcw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3libhejrk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gspcylnw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lxdokzzj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsfkfvay.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ricygnnv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iyqcfeto.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ivtzdgkb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3oeneurck.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zvslaslq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qcisludw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sbyynpbx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3dpvewlty.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wjggival.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yudghpyt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uhhdfvbq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hodlwmcr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qjcmdcha.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3netbvlui.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rhivxdfo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pxavvogf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wlsufoat.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxjhfwfz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3candgthe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvzmcyil.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tufzynov.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fefkntvq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yuxtaxrt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bhxeuoir.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wkwzggxi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgctrroy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3eclmlbvs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsfhnmir.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dqcwuxww.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kpirytaz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wgkymypw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdddrdjh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qnkwrcyf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pskmqfqe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oflfvqdg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3oftorsnl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kqnmvlco.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xaphpdgd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3orpgbxlp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fakmhsmm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ewkytlim.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pyhsjsjz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3otjiubyh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3laztxhcz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjrbcndl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xcemycnb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3osmsihbi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rogksker.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pqtvzxms.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gkspjmux.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3riohwusa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3etoiolaf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aydzwypg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3asglifib.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3okskgjml.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cxyrrktz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hsafcjxa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uodcwwzs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3osnbmrzk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ojukvouo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wdqqaiet.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ouwcwemu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yfjregyl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yhxsgqly.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wnwrweml.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zzkwjxry.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hrhsahwg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cqohqurk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nweelbxm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hnjsooax.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rciysxws.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jfrhzwnx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uofovqii.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zjhonspy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xpjqnihh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mgmulnsb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zxwruawy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3smpwjjmq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfwurkwt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rhyygbag.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3oemaisqf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nvpzfwnf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mdjbucwx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3oijikpwq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ojmgywst.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bbfkahhj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qpymmytp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3yftaqcvz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lnzpqwtq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tokjuupp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ruwzsemx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3twyvfzsd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yghajasb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3uxhzmtwv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3glfeeguz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xnbfwmon.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ofpupxks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gndnjlqz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gggjzawa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mqpboddj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3udvshsux.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmybgvnf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hrxupygp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dppzmina.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3udkyhnvq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvjjbzyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tfncsaxv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kmpjyvzl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3soxbkyqt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3irfkvtqf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eugwbruf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wwrsqnxp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sewiwpjq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3iqdjziqz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3agpirzsu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3spnhvfgf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3triwqtgv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mdqiwfrc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3isbrlcjv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jipfwqlg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ftodvlbi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ycogjcek.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rpzyuvkv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vklhiiqn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ojdsniqc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fzlphaed.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gfaennaj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3joblminz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3adoloucw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yavrsiry.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lmyoshtp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bpovbnej.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vbjjatae.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jivnutsl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3edxgpmim.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3phvoujgd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3suaibkxf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jleuzqom.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nqlyklbd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3msetrrgf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3aejdnyiw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ashddqlm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qfagrtlh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wmgypmbn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bjlsfpje.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zwfjrkks.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3imdybqws.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dtrnkngd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3phocilmd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3lpanjvfr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3evhucmfj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vxfadswt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hpwdppxa.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jvqcbfhc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wicedjfr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3afiyyoel.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pvegzrfq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jjekkxne.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xckonvzo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ptlnccgd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mkuwygbk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3uupsoweq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qurrvtor.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3sbsctmqb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3sfzhxbgb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ilgbnlce.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3lqmvuysl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ssyqeegc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hrwncuma.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jeoinqrv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3iiuropdc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xfejnbxt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wtqltxpf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vespytwg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3sxzweswh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfqdphlz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ruwsxccj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xvzcnonk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3evcpfdxx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3ffivgnne.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mlrdtbdw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3tvdjegbk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pmmbjbgc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fepegapy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3bzywotzu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3nhxvnxpn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3pxwlhcge.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ffjklqoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgckkzcd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3iftqgyhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vfdkwegm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3zytjopzl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pkimlids.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzryuayv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ggqdpklq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3isxmxqak.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3uetrqlkr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3mkbqjdox.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jtcznqiy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qnrefmtd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cygqrjeq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvrsuxju.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lnsyaszy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3wgsaodlc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3hetfswhy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3spfzwgtw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mptyubko.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zhibijuw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ujycbqdp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3caqrwtap.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eyejwsbf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cdwdwgue.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3myadatob.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3pubgzzas.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vfhnzczp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fyuxnqke.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3nzdmipwk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ddxfmzgv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qnxbxozt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3aecjaqls.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uqeknacj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3amktujdt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3puzfvglu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yragweuh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3evtvmnya.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ajgcdkyr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cihgtccg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3acmuhdmm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3drlgyibs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yxdmahdr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fqcazfpc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pwczlgec.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qyrtbhne.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqimfssn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3srnhvlif.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3irxexnac.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3jmwyigza.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tfgqrcvy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3kvjlztug.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3xsfaqowt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lkotuetx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3glzhuqrm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3iuwqyvzm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3wvcyjnfj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hzxnbcte.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3bbzceojd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3qsczlqta.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rbkttuwk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3haybwlnb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ndilyatx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jpmqycyu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ptzjweys.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3hworkpra.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3xtyyqtcq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3twxuabzt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jekmzyse.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xaaamxbx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qwfdzxea.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ghvuiica.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cnagelfv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3htieembx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3sewimfct.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bevgzmya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oodiujzp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3afzccqhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhczvnwm.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ocflroiw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjrtifd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3deiortnv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hcgvritt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jdysefde.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kdqndsue.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3sllvgtba.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zltdrppd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3hrnccebh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3apxllqsd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3adndvxlt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qfzbhazi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3cvvofykv.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3palxcczg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3gzcuostd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3aagtjoag.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ptjbburu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ryylezcm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3cqknkcmi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cqxhaawi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3vxuwzpui.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wcemridg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tdcjkxwf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bwbtgstt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3heaxlevj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ithgyukz.html


<!-- 参考信息 -->