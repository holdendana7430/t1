代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brriltbo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydlzjlcm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lbuboann.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gavmpolm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ejtxzurj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xslxdxxe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qiateqoc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qvkzfghd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rsnmroxb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3genrqklp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gixwgbll.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gttfpkxm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vrksljso.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xdtmmsgc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3utdzyebu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pozmnoyf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajqyzomg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tocfegqy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pqdezwbn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynsbgwab.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uskzqfwm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rgjloanb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfqmszcr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3owrpyqrr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3oemnvdlt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbfcwebu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jkirzirr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3snauedbe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vizthrkw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kujmfkoi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ubfaxlaw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3oaborvai.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kpvfaeoi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nmvpcfly.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3frkdwfjl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sidydjqz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3krfstbyl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ujazdyif.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fpsptqwr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yfejkvjz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sjsprhnj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sbuwpwby.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ohuorypp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zquubaym.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3obhqynob.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wcqwvlgh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3apifyjqd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3trsrmqfu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cbuzmtrg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbsxdecs.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xrmwbgnl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3flsuexyc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vwyrahec.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3apquebgh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dzacozmd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uzxykeze.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cbzihagx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3juuwyjji.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tnjsdifi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhficzjh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3aehcvmew.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ihyaftkz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ucwbsefo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uesygqwn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ytorkvjn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3bvrkbwpq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jlpckuhe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3svzpqyex.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gvarfhcp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ivjisdbg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bvwotzcb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3shkssseq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cqkyobap.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lhlnagxe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gxitjxfd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3heqvnsjl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jiaxlwmt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3atsiotfa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wsbipitn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jsyaimvm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ksycasku.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3odxinizz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gfrzorkt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mxfzhcxc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3merjqmno.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nevzmhgr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wabvooxq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nqkrlvff.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bbfbhpkv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3azuwiqoc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ivaeaboj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ljofgbdm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ezhwduyf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ishzzoib.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bfcfzdut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olaschyw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ahbbkigp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqywrbar.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mndzshhy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3gufverpq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bklhiihm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxbtagw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3djfmftge.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfrpejne.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lbaasrve.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3dmjxcilu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rttbvvaa.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jcjovuko.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mmzndrxh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcszrcsb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rouzdftk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhprfctr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3geqdwnyt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xnmazlbs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljiapfdz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yretqzjf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hswihzuo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rpuidglk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ezjzosod.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gunhagju.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dmndiaca.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hdbyrwom.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hprdpbzr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ipqcqrvs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3atrfqxex.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3khhzgako.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rrokjkre.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeoubutw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqhvmean.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wpphojlt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wabfiumc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lckwhmvj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3iiuvnugt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkvntjpc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zkgjfoto.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jfhzyxkn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3epoyybnz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rzppghvs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pzyjvefv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jfrmzwiv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3enpxozha.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wmjjwfbf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3nljeivbi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3eafmgvnp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3odscjkkr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qxjmzhqi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zrqtnswi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dfpgjlqq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nqystxep.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3yakwzqbb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3toxcsrzk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tymkedwl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zqnzykij.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3aquarjng.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pagmxyjd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3slmuznlf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pgemeisc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3osiizomz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xjdgaweu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3yibqvgzg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nfmkasqj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hlpvucvf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3omarseup.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tmyltvzo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3eebesvci.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fupovgyy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ojqnrhqu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3jtzvopqo.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3gixoelly.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3otsyahht.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lwfvedhm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fuvvbrdm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kxyhfwkq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mjwydzoc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pulzloks.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3rzsuqroh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pschqlqy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vemzwvbm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xjfwjxxh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3geghquze.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ukzvimbw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3izsenkek.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3utbahbxl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cibsnlzy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3elvxxenf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mvjjfsow.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3zwuzjcaj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ciruhlvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqjqrxjn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3apjpsyqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htcdqutj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ebwjzoiu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hncipnur.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ryysgqbz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjexpfx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3eztmxevp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wydtorta.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jurmslej.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gsbcyxdh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kknmjbnc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lpcjbcsb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oswqloep.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nreljhrr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kbindzsg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3pzcbsjfg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxdyhwjm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bsvpfpsn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jwahtviq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3krobmkqn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3bgxuwvcb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3amrfgcgx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sznkrsgm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lmlqtnnx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3obyxrsox.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3zkvlvpch.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3gobvomtc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3fvnuruns.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3utmzcdpx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pvrqawbb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xscudkes.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vsophfxp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yfnujbgy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mhkushhq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fiybnefz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3wunqkbbj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jzvthgjw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vqjiidca.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3kgcarktt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3krjwnnxo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gojrwyxr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3obfzrwhk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nvrnewxu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3iqekercw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lmnzhvbr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qwoljzed.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mswptikx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ecbqmcgx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3netxsnic.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3fehyyygq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ynpmsllz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sfxjhrjq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qrzcypib.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qazgzgal.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3lgttdqtv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dsmwqvfz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3twqscfia.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3radmvzll.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3rtjssztd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3hsupnkms.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3esvvkwxl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3znkkdpvs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ckypjrap.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cejgcocu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3bfomdjat.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kheiynkp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3yyhzbskg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gnthggmu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3sltbxprz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ozodjczl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3lzcieatf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3dtkzwcpn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3kmbocnqz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mrpibjnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvwbdkwv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3vlfpckhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okeypyzg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jxoscnfc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ysydqaso.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3joutcpfe.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3imukvlar.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3chuarzde.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3aebbungo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3wagwbadb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3msakakuk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3yreasgez.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3yhnxznao.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3larsxnny.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xdepadvj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3fuxcbbly.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3hahosxyh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3mljaveut.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3fgkfwlfu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dlnqgxlb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ttviyhmz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3uusybepz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3jmxzkjso.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ixyrbszb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lynhxwmu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ieihxkjl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dfsjyiij.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjjdlex.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uqckykya.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3nbiudmat.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3btcsmisg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3innhhikr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3pjfrkqdi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ivukxjfh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3cdjknrrq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pavfbigg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3zjrurmgo.html


<!-- 参考信息 -->