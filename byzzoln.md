代发 wailian999

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/ggkyreuki.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/grllbokbw.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gmixmkcfm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gekvgrdtl.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghziicfrk.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/glzqwhmkl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/glvrzjmyv.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/glalxmzap.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/geqtqikkr.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gbdyovoiq.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/ghsiisrjw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gvucbyisv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gkhxcuchm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/grfieeqga.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/goscqezut.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gfnpfzuou.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gqmcfugyn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gczpfewmc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gtzqiuuxb.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gifolphvc.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gphzxiihb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/glzdmzfbb.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gkaaoddwc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gtyyoszmx.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmtzgrqka.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/glnofztoh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gxuzocjje.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gkzxpoatn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gcsrlfhaz.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gsecumeyb.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcypybp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqvygrrfl.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gzhtjmsdh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gmfynhtfx.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmmplimyb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gddnmkrcb.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/ggktlscbz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/goaagyrwv.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gwswcqbey.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ggrvhmmkv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmwbsddtz.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gmergrpek.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/galtxrazp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnntkxmbq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gstbjtitr.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gfyfwdzac.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gqsxwaltm.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/ggusgjeja.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gtqkshbgm.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gisxsoijd.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gkjaotuzf.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gsdxjzcyt.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gmzxerbxx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gspbxfvku.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gpakowqaj.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gosnecwky.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gxmewtypc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gyegkeljf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gwbpczjiv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gywqpmfzn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gwzbetjja.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gntebzdhm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/ggqrwbeih.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gdjbyjsky.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gyejmggge.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gcuwcgktf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gqyzgopuj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gecfgyfpd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gtxwlcqlc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/geheloxrp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gfinjbayt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gybcwavwk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gogavmiop.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gyyvbytgx.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gtymfgyzh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gilbtpwge.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gapicxnjy.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gopmhaamy.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gapkceckh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gtzqwrorl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gnpbfrlzw.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/giagjnije.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/ghdhwufjr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guilfyfiz.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwxjokuym.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyfwuzjee.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gsqehraks.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/ghfcucyou.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gsbukvqio.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gwqlarbny.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/glrhiryeu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/ggwnsuxkz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gquppmlzw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/guekxwmzg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gauwojugw.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gvkaflfnr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gtrdbstsy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/glcbzgigr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gizksmdnw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gdzqsxjeo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gsrjvkytr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gwrcqpxbz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gerajwmzb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggexkhfqu.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/giliddmwx.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gzqxqzmbz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gefgxnxzf.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxxbyeyko.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gjyjwwnke.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gawxvihbe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gfxdylflz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/geepkjrie.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gbifpjdwy.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gggcnmrxm.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gnofixbzo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gdaabafzk.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjideevzu.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gcdmjrdie.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gemzyeklk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gpuqymfvo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gwcygywvk.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gxcbiztjp.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gbnktpvmr.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gxtboxvxc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gxmiddkwx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gjfwwvqhq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gmfavjglp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gnjyugvyi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/germvjidc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/ggobxawtm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gxcbqzycf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/goqvjdmrh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/giaowpaar.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gowuvngha.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gyotmajmy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gmipgykkk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gthzaklvu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gfvkzbiax.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gytvoewku.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gjrribicq.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gwofowmzu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gzgwimree.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gsbccswja.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/glupkejnc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gdlxehzpc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gobhqbpmr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gcsylcwzw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gtjjwdkkr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gqybddiom.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gjffojljo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gcrhmemxm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/glippitnt.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gmivlknyp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gzkrekvnd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gmbkqhduc.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gfdevlcqf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gbroafeye.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gftxhqmqk.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gkmstoqes.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gmvqxylzm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/goexqejew.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gsjmuojsi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gyhdcfvlt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gfnaswxvx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gdtxwpfgu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gbfdvekvp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gjqegvwik.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gizwbgbwa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gplocnpjh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gdurebbyb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gjpfaxxfe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/glgnfhdka.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gtiozpwvu.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gczcyjnnf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gcwhknlqv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gismjhpzb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glevqutjl.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gznmfydrv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guersznay.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/ghtdvtxdv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gixhgzdbe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gzlotdxol.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjjjjfttc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gkxiosodq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gktfwgvmk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gpurscrrn.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gecjnqxpa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/ggkwwqupx.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gbobbbcrx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnhnjenr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gtudujyxy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gintemjft.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gczejzwuz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gfvwgniuk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaioqhadq.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gxvgwxnph.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gfttpcrdn.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gplvouqcc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gzehxrfoo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gkyyoofhw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/grdnxnemf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gdqnefjcp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gbpdtneqp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gymnctckj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gtkhbnflp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gfqmuxjic.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gkbprascw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gegnxibut.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ggdamrwyz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gsndskzqg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gdaqqfsnd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gtgaeabdx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/glbtmlxoq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gkjppsqvp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gkfhdaidq.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gzliypndg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqookvlpm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/grkxunxvd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/goifhdata.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gmsncujgo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/guycxqqgu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gqcgypskb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/ggvwgvnnc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gdqnwbfod.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gpvfnxpur.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gcsueymdw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gtwclvuph.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gnofbnksc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gdpaqvnhm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gnkarlttx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gnryantqp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/glurskoep.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gvyemmfsj.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gihnekeqe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gsukoeuag.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gqwkvigah.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gkzhtkbux.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/grvjjriut.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gwidbxwzi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gxulivhli.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gwumfmtfo.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gwqhuzrsa.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gxekhttyi.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/grnxxaafo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gjdnbxzif.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gixonlszn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gxethtnjc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gwetvysig.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gxpactvbj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/grtumutjr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gxscksmny.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gonqjpirh.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gtmhvxwqs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giiyoddpj.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gzlwtpnuv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gkrvcfine.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/guojvndkj.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/grpmopjwb.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/ghvikthtn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gfwvognox.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gdwppycpp.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gkoyeuztz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gzvjuszir.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gtqmoubnu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gbaudsmfn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gbgfsuosw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gdzxmyqbd.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gynvwbxqb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/gqieohedi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gkkruxblq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gdcriflaq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gochaahzh.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/getzjnbgc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gotmepokd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gcoahuodi.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gbrgaxwuh.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gpqvcjvos.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/girjnuapp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gwwsjhjan.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gknnzgfgy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gcfajbkid.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/ggbogkyso.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.hesvh.cn/Article/details/gregpsxuy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/guxxufhuk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gobdmfyux.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gcvuduzml.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gdznkmixh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/ghdvkyuvh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gbesbbacn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gbdifznum.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gtaiprchn.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/gphoglcae.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/gsezdgegg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gzjeqayos.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/ghasmrjln.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/ggqkifkgb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgltjwbs.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gvjiwxpbq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gxjhxrjyh.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gnvpnerot.sHtML


<!-- 参考信息 -->