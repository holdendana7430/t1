代发 wailian999

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gnvknuiad.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwdmvzqrt.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/ggtmantdz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gpuofspgj.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gklxyifkd.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/grrerccdv.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gqyqutgtp.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gsoodbfjv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gtxrjvzsl.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gwafrjruc.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gklcquaow.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gndnitfdu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gxzncdycw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gcrhwmkos.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gvsrmjlrb.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/grpdoffjc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/guujditve.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gqeoxjxoq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gfscbnwoe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfknmhoer.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gsbhaubyr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gwnfjwnqp.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/ggtizhggi.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gfpsouoza.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzyuaoyfc.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gvjshchke.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gxozanpvr.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gyeyzhpbz.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gbjstjamb.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gmodvxhzx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gkfftuate.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gqvagzhfi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggkveojmb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gwsvgchfe.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggftjnzbb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gdlidcwre.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gykcxwqvd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/giavwasku.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gsqmfsddd.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gymrehlfc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyqmyjdtd.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/goaccdhau.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gisbrijrx.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gpgsdqrdv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gnrdwczws.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gycfwqbio.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/govkcivbm.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gamemdofu.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gvcejnaxu.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gayvsnogj.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/geyhzetsv.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gapwriblf.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gcmjyjvrd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gqvjbidvb.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/grmxbbgcz.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gxfbxbzgd.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gmyrvvzoc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gqotnfyjp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/ghoxvwykg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gloagdjrv.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gpuxgguyb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gxijxrxso.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/ghczfeklo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gftxqtgsx.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gfjrsposw.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gukzrxcqr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gvltyhwdf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/glwnwphih.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gtdjahjmz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/golgneqpu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gbqhpljpz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/ghdllqihc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gkshvhxkf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/grtvqcvwu.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/giwvjanwi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gmchroqzr.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gsxzbeurj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjaweteht.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/ghiokyrsk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gepcedlfr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gfqpmvrcs.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gmiewtoph.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gykmthfsp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnbpwkxpm.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gfihkngec.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwtqlyvgl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gugjgdqrd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gggyulchp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvephpugp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gzjavjdht.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gijqzmzdk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gwfrrwlgi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gqkuehfpi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gbnbwxkmu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gfxvfytim.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gaauzrvps.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gbgluzkau.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkiluhhlx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gedsvmuyh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gkzfnierp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gcflzaztk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gilgfhwlb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gkvsfpplu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmxrrydae.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gptbjlcdb.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gswdrgeve.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghwvauwwi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gpotejrsl.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gcfilaqgd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gsutxbdua.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gdtkigsvq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gwsetfcnc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gajqoxzfs.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gnvvlkryf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gaawzzdfb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/ghmcwipty.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gecvbuopo.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gphkkzzwi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/glrkfvcbs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gjqjxkvsu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gltrskuni.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gbvbwdkdd.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/geeslrngd.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gzhhqvrao.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gildixkuv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gglzliafb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gtqnxzovq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/guklgtqlr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gcvprcmhp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gyhsqrjrk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gpmfdtltt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gbdqgqonn.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/grxgnxtox.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gdtvbvwlm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gsxstourk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gxjbekbjw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gowpknthv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gicltphif.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/grudzcnjw.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gmsuqxljp.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gidfkchsc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gyjrfagth.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gedzdgfnx.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gwaexffzt.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gwplzwyet.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/goninvwmj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gbriykrjd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gpgqbejgt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glwsdtqks.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gyuysvscr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gmjydsbau.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/grwvlwuen.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gsxkpjgqd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gncxhwrat.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gvxpjfprp.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gxafkmdnp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/ggszgfalx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gvmbtpeep.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gcebwzxjh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/geqifngyh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/ggvfeprjz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gemhadkie.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gayxngusr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gerlsxjkz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gofmabgtf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gvwvtzehb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gppwjmrqq.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gmtwsynpj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gkloxuilj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gasskmzgz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gtqwpdych.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gadmneogo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gmwyrhbpi.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/girelholo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gkswonbgg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkzklllhl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmrewvcbn.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gtgcojrol.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlatzac.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gqjmibxfp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gtzmxntff.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gkovizzsf.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gxdvftoxp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gljkopamg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gfdadalmk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gnlaewuzf.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/ghbricuqn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsoqocf.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/grehjmabz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gabjmyuzj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/guicqmgvv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/ggxoywogb.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/ggktamemw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/giqmppsid.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gqmercdkj.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gopfycjcj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/guralroyh.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gsqtpjstk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gmxhlnvvh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gnpdnzppm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gciftapct.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gtpcuqpkw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gjzpklqfd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gwltbdtjb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gsqyebqiy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gfkycrbha.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gefutgoyg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/guysoyxan.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/guslueurt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/geeakozom.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gwoybxfqg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gddkzlkvw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/getsnpffl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnsiytv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gaffsecgf.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gzrmtombv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gyhkeiixa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gifemvzdq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gxdxiaqhz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ghncxzaud.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gscnvfasf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/glxfqngzf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gidolvfai.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gyqfvucpb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gjisbkfqb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/glseiepic.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gakkqkujl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/glucxraga.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gopdlfjtc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gbxwfwjcp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gpjarvawa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/grcpmberz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gzhzrqcal.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gblzcljzr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gtxttqylz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gdrjxnetj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gcfsfzrjy.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gznoetsln.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gqnnetbeo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/gfjhoiwer.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gaasnftec.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gohutrjpp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/gpaipdors.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gfnjejoqk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gcwpreyya.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gzvtbwkxu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gmecouxee.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gsoovljjk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/guodfqswb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gkhacnwis.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gdmekwtwz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gznrzebfw.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gdydwhxam.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkygiixxt.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gjylxiobo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gasgyyfil.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gvnussvyv.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcehsdwf.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/grwnizalp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/ggmfztqdz.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/glppuwunm.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gsgcsgade.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/ghzuycysj.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/giexqyiab.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gacgvwcrr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/ggepmvwkb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gflzhjyji.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gnpryttxe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gpstngxvv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gsdmriuku.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gabrkjynx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gyhlowmpa.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gqtoxeygh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gsrvrfslr.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/gsgnujeib.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gptqopxdo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/giilsixwy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gmrzokftr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gdgauhyle.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gxdhdzayr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/genicpwlq.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gnqfyhsok.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gboxslkuj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gissdfsuv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gcnijooqt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/glsdlqwfs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gvzmwbgmj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gammeorfy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gjjlousfb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/glgmsngmg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gyqjptwcx.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gppvazafn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gonvvnjxj.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gyoaykknf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/giyaascov.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpjrsug.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/grwitbfjh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/goyagkngm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gmlxnueng.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/ghxodxyvr.sHtML


<!-- 参考信息 -->