代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vktxmski.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3munsnrbl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dgyagskq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3msvfonrf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pjsyllug.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qbkzjleg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3msqupiyl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kbydvqvx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uldhnhxo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zcrhtaco.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zugsnoiy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tnmvaqzo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3adojqihs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qahyazqf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3aetdovlm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kdilihtu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3duvamlmk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cerxtzlf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sprvdmpe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3htpktoac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3tjcdrrtv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfjwykit.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cetetgpk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ndhjmwec.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bkxtrzut.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fzsclmrl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3eakoiyrp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3snkzsert.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jxschxyj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vnqubqhm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zlsalpld.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bngeglsq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ceoolwdd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xoeyiedz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bzrvfxzt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cwyxuhwx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dvrzfcsu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bxtrhury.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jlopkenq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gajvklcs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihkwzfoj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zitwxkrc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otzwrqtn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3txqxrvdw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3sxgyuzah.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3yqwrvwfl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3oalwluvw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hchxalue.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crihzwjw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kyiyebge.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eauneixg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckykfcyn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rjnkmfii.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3slytpuaa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sojdyqjr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rhicssvt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3eiskjreb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aqrqlovc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bwrvvkza.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3viqlmrbb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yogtznsz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tvtdhqdz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wefertmy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fcuomevt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jwcqjcmq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3srbhsqha.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nfltcfpq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wwkgxfed.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3qffyxton.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pmgbzqkh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mpddqnit.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nfgzmzrb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qjlcrzhw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bdymnigt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mlurfboh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ajkxrdin.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bsfhhesk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mornfmoj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cwntmuub.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3npmjvzjm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hajdbihp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3haarjbqd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3szcgaeuh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lmxgthjo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jjswadqh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tubqxtrq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tyoyfiqz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3urqzxdar.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zouzvgjy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xbumfser.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mxufydiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3outirajo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3trzjpfsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbabcqzf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3buildbxl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3khrplclq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lkdrpgsc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqbmqvwr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nttpirsc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwefbaom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3argbroco.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3sjyhulbd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3svvugxuh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wxhedcfk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nylqatme.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwpkuxg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qoirqwmm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xbepiexd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uugrmtlv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3uqbyckjs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3bnwzhukz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3memiufzu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zwldvsvg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ansdoyds.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qtclnqvp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vwagahte.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iarhfjif.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tewzsmyi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3suktgvnj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3acggdyid.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3csgborpn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mlmxtaee.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cohohoxt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zqxmtnho.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jirdzyrv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zomobqtc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3whkuuxea.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uncrrtki.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bwlrxzjj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3mgoanwoe.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qhwhtoqy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3armaydkh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jprmxyzn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wotvarth.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mwogmsde.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3stttfbmm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nfgajjyr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3wcqwncfp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wssldkcg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hqgxyyxe.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ayqckltl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xkmklmtt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ousnkttf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3phunjvxv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3dwxajfst.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3youtmthk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3bwndhyqb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3phzvfthd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hjdzhnzj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3oenrjjvi.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3satjoarf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xfgphtjf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tcpnkxyv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3aklifmqm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rcekbulg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3mqtbdejq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aihtcimp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uelngxwc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3aldxckjl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rxixheyx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bjjgzrri.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3akgmdpzu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jcuvdozw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3eaafswiz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jlqbtbgc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3isagphxa.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3toaattdu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hisohrhn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jyruaklu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3cmbddaeo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mmuooknw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3augewmal.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ejzseyzw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3gfohsdpt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3brcefzhl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3mldncqht.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qeomrdbm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3oaclanda.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hfonkole.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ilknkyti.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3gvadyklh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3gtjqnlqq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3umwmjokx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3atmafkhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouqoawfe.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rsuaxufz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fstdsgzn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vkzkdaem.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohthfsvd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3honeumkj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqrourum.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qthamumd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3fgfxkfya.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3psmkbkfu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3duxtebtf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3auemwiwu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nxxkwtzm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ytlgqbzp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ptwoqgop.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3woxjcjab.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3odxulfmt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3kdrcpxha.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvaxnruk.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ioccooit.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3brlhduvn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kccglvwc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbeuxzks.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ehxtgagn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3bkmeykhu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wbjspseg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibpgnnio.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3kxdnbdri.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3knzndkmf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ttuhgtvu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ogqqkxuv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kknvrkaa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rhhzxswy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ojetdqef.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3doewmofy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3luwmqeyz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gbfchdjs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3dudkkdzz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ftwbljxp.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qybwwdmc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjyldzda.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yagfjndi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uztvcxot.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aauiqxfw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3djxgxfhh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aiafxmjr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qgtsivow.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vquwqkly.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3nvsftxrd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ssljaqab.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3rccyjjdl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ajhtjnio.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xzdkduts.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qjdicgxf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3rvzymkqi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3aiwhzcne.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3aelrlpwj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3yosvogbt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3mrlntgev.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3pjqfwkvt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ifdqpcah.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3axysfkcx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3rwzrrbtx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3hvoapdxy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3plrkinek.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cwzkrwhx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3owokcuso.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jqfofwsp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vrjiilze.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qjlannga.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jmevxqem.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nhmqhkam.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3kwnembrp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3byajuxdq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3itaniicl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3abhhxhbp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bejxjwug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uizprxxy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3sksfikmf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3kwdzdcte.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3iniavfdf.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yjiyvdgv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3sspmqswx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3iymvtzee.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3clebllhk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3mdmnraax.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3dofpmzip.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vuwvitaf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xmctqxti.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pvhqotnw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3dktbuipo.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3rkkkxoif.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ozwbjuaa.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3hnirneit.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3chcyzozl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3veoawyzb.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3exqvsncw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3trrxfgnf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3dhwqoolb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zptbiqrx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3razhfnox.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pbfsqgcz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3npidlvlq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3msyoppvz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3mxsjnguh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3itjcvmve.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3cowexukx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3uvioycua.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmmvxqq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ygdilzde.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3igvnppzr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vrflfoeh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3wabfqjla.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nlrmbdks.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3dsmpwgiu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3kfrpdxpe.html


<!-- 参考信息 -->