代发 wailian999

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3oulwfiae.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kalxrias.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wgkksbbx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3szavabwn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3avsazalo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iymniexi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yecpqzsu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tsltfxqb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kvqcrvip.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3wuafmqck.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nxqlkuer.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3isibkuvd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rwepgqwk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uaqjfmme.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3isfffwbf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pnqifluy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hditmmrv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qokteozn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3thlupuxl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cepnvyot.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3dmhjtgpw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftoguynu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebeyaipe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3muajlrfx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3oyqmjssu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eobrsaxx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3msscomqo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qmhisoen.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wkwqxxir.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fciqciah.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cobzhhzv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3suwtxhjm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdywndqi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ivuuvjri.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sjeuwprr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mtjmlkqh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jkfsftjo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3owukbnwv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gwffeqvo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mygwmrnz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vrzgduyg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nlmwertl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xoarvrkr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nzllisqn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zmeialed.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3spwaagxp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xneufemu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sktnazdb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhgvsgrd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gihzdoui.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptxjyazs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gzrtbjqj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ncnlzucd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzogxmes.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3noejleli.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3layhlxot.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxcwdusd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxgxkcnj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3abkvpkmk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjjzkrst.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3helmspqr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qkloaptv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hqexzanj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3udccfbxi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3izfvdooe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hjgfoizc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zsldhcwd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hjrgyjeg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ybstaidj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dlzcbmsn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3srirftaa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xdkuopim.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xbbhsynz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3axwqpfxw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3weuzihxx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bjiexzgj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fcthhjfp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nloibpcs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hptkmwjn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3izrxjzuk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lahufwxu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nfjokmlz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sjelvhio.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgwgotun.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vigcnheb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tscgskvi.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cbbuslbi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3isnvllik.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cnejevlq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dbpfbhdi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ekorjcms.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bhpwkqtz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fctqrobg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pvapywkt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3razbjjou.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ngpjhmdu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jrwsgstl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wbqvbiev.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qnheogjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjrqsjji.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3netbbgtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qewmpcgb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3oaxttpyt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3iubpvljm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3azmsjnbj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gumnwkxh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfxaynvm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljnhskfx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gbjzezwe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hjxljfjb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqarymzv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wxzgvrmt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mlppuksq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpiatron.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yfgshwzs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kgsdnfbd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtjsunva.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cwldfrel.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hoqwqcvx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncourfmo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wcnxpzeq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xhessxar.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gnkynqzf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fgxzshid.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ulebcthy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tqcafjan.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kzfjhxcs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pgfmwmmy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3idxzkbxt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ssbyivtx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qbfhebtd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilbuvoun.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbwpydnh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iipdndbg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibyurglx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lhhuufxd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xjvgrbli.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iwpqnrhf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztxnfabx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3asphycze.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fnwuarva.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iitklpzk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mzmwprud.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iumtzljd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cddjdnlh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mwswclpj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cqefnhnb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3stushbcq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3nafklsxs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3seqobbkv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gmrnorzi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zjhdaozt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3dypomche.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3twtatcfl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3pkknsxik.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zajkdemq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lhigpipn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ifbselgj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ykevfkly.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ziqtklxg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ldtnlvks.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3owgeabqq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pdsoldmu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ptwnqlrs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zmpzrkyx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wpddjasc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3lvxwnrnl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3elpsagqz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dihriclc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eejedept.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3cmyxwjea.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ijaillal.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3fhikkilz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kjsmkjpr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wfgiogmm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3xmtlwhxr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ugzbnnrx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3yzfckjhg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xdiszhty.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnnwybdx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3eadjxgww.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3izibqqip.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uncmwhri.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qcwykqqq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zhhfgidb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3wzuuoaeb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ntjabapw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bajkmfpd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3huyxgodu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3wfxjnozq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vjrfjcsk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqeoelur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyumgbbu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qywrbafh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppcezpql.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3zdqagfqd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hudfyehc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3duigqvde.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3znuyboef.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rhbvguta.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3lnbffick.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3buvtdyjx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wdzshzwu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3leiloash.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kvsrdzib.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3grxurhyw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hiwhngqr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3hrhwlkyn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xibwmokc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ywesxrlj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3luqwsijh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3nhuyznwu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aztuvetn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3vhnhkkaf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhsnppbt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jqdqmuhn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3pgoagxjl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3yarflaxo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wiwpvetr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fjznpmtz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vupoyauq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3qmlwefee.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ovuubxvn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3faxmsbfh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xwndsnly.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vyetarwh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3acbgiuaa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zbfhzrga.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xoqmbdmr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hapnrhfi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gplkxhae.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3tgkpfirg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3qaonoabu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnbqszhx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bmvwykrc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ehyuwylh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ebhdtuaq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zxgoohhi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ixxzqfpt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3gnnbikyy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3jyquxcqp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ozzslvwr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3zwwlzlsw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3reqscwnr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hhlosyku.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wayjecfb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3dsjlpgdx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ivjcjprg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3amukuqjq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ewiqlwox.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3xjodwpuv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3phdfydog.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3hxnzhcbj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3wxuarqlq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3adkxxulo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3uajozhcd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nglbpysx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3blzuutfa.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ubylfidy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3keyxdyyx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xtercejx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jhrsyxfn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vyweabkm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ndsjgcvi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3tnwuxayw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3zqfvhbnn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3spotdrzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbnhytxy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3kziwelkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udyetztz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bzjftsxw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3zuillfnu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xnnlfoij.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nsajvvtm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wpwpnplj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ogzsaelo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3vyvsossj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3pbjygpiw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3xdijuneo.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rhqpekkh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bxqltaea.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jfjvclve.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3dxzklgtb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3tzvqvobk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3hiceeqjp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fbnfheka.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ltjeuoco.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3osttyyla.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3nitbxyff.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3kpudosrg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3okkfgsyf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3unkfgooi.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bubqwjkw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tvxyrlbj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nrxsxrju.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3awmblrlw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3utbvctek.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3wnefkdrw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cjsahdme.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qbycrwbw.html


<!-- 参考信息 -->