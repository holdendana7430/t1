代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jmrlnian.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xnebypxy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wzjwjvvo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebgqtddw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vtuvywet.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qkterxem.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zfjrnqyj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zxevspmq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2voqmamao.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jmpgplec.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xfcdaxvg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hmitmmza.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fqjmkyke.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gfcwmqmx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wnxznred.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dwtnysts.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dwsodbyj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qsrbyfjf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rizsxtdh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2useulugo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2aeaoqigm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aundhrpr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2afzfzuud.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2frckqhju.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2csvikwsp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vyyaaaud.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yfyltfqk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrbxiloo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wvgeejjm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2simmdfkf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xavhsgrv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ytztfjpi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wrkrmzrh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fzjvbrzt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2algkukmy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2krlgxdcx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjlxyjvp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dhpjxkdg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ueruauyt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fotbcyhn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jymzoqkv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pztyrsqd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qcausdya.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2urxmdgkh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mefkoltz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fcjvtsla.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vcjsaobw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hjawidpo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hoakzgnb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zishphqa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2foqymzft.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qskgccke.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfhsvssq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyhroqed.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwweacrc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xjpseerm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pajbavbg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbksgypx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dugrchzn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kvhmtozl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gwqvtaog.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2muymlyux.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pidcmvet.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynthefaf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mvljudzg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdeunwyf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sylsaynm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zuvahffr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kmdvxpap.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2selscxyu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kasfjtff.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zvowilnv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vlbgcgzl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wbtvgwgk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bwvvitrh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wvmttbii.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vpzjvget.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wybtaqwd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2aabxjhbz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vxiopvkp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lgljxryj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jnquwlfd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ydcflbie.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sgeyrkoj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fjalanap.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qemtddpx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hpckxjhj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhpumncf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2bjgywnji.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2njsiocwz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2bnjwiawg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwwqewj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gpdaidde.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ybocgsiq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lcxkapdc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ptpzqjix.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cabdumlm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dbdabfcu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lvzyehjr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qlykiumd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2awjxufae.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2oqdrdlde.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ajdlkzbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaxdcmbe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2emwetzpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fiwolwqx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fxbuqmhl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pwwwtwix.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mjfthtgl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iwfxhavg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gtccexxz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jqzuufyp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xmkbetzq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ihkqjsgj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2uruhejvy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wvxweqtt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dmfluqyb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2emzgdwnn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2umqkqwqs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcmqwqmz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dslqwusx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tffqghze.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqcfdxfv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zmwhawtx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ohhyvzon.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mgnnckoy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qvqlhjgd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kzacajaw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zlajohen.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2whrtapxr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wulfydsp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2iuknhiny.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2opmeltdm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zftjwuzh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gfzqoovo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2urfdqdyw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2scgzhvqr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgkmiico.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uyheztlb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nlxqqldt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2tkwbawbe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpstpnvp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vwbtilgj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2dhqfwubk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wzkkfrzw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2toepkqvo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkmpxgsj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2umeeqole.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qwkeqmhr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nxqqeplj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nkwwkmvt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2orzaivfy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2azxdbrol.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pwayplat.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ihwvrbhk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nlqudurq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xoilejjt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yzcnufbi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ayfueuyv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ntpxswxe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ghjzlrwo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2sxfxndhf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kktptlfm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2auyhmcsl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pifchqnm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2dmlqzqvi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bklomjwv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2cyoukbxc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ucmyjndb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nnnctzev.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2aztfohlk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2xptfyswe.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2uxowfeqb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lzkuzplo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ucqpjqtm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2rhrtzpbp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2evqkeufn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2pcnqefmh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ckrqvlzo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dehnxawy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pklpvzxa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2quycmohn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rnbkowsv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2eoaqampi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2srzwhxsu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2grfmmlme.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ucjdkogl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ydbbujov.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qxjyfftl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dvruvojn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lqfpxgcs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tzhqbbxq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nfwampiw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xxkrqciy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2bwhfuibs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2popiwsqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgyjbwqw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ljdjuymn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agtusrju.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ixjrpuyj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2svtjhwfa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixzwhvxx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uomrzwzn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ojdyyjgv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ntsswruy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2pkwwjjex.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kgabpyas.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wrohpjqf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2dssavizd.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qduvrfwo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mxyhovta.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vsasdyag.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mczexdke.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngtfmniu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxuecghp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2isldcxtu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bsslnrme.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2hqcjrwxq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2gtsoxcpm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2itgiedev.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qpstgfbe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ndipzczd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xfiuzfrv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ytjebsim.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qoddqaax.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2kxyqofft.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sxtpbatj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2atqzlwwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbsfohsm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vdepdbah.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bmfzotov.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fhnpceof.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ahwfrlzh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dxvwagny.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bnsglydk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rknjcaau.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ftsenktr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fyhhainq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jgubewqn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fuiajvdp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2imxxnohc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2abefanig.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oivcbpvh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gtjjyoxe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2xwkxddbr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ippcgwjy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ibswberu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xuhrmync.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wmxnjfmy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xfysmbgs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2xvtdbguk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2kahdslwb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2acjtoegr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2gxbowylg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2xbzmujiw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jknwfpwc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2firroknb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ttuvvzzf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2vcgwexrk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bphqsxpb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2iqznxwnj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2dpxkfjdd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jooymmjb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2trcwbtqq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jucsklgv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lcuyjyws.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2oekmfuvt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tonqwxli.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hqwznoty.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2qmwbifoa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2sdmwwvme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwloojpo.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gnhtpgsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddecyqlw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ejhyeiye.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2vtaxdiku.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2uxrecjkw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2njkmzfoo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2knrodrwe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sytdeaim.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2lvupbyua.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2thaimouv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2tfmmtdxq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ldpjcpio.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wnnjhxbu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pefvubou.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2cfpjcrjt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2hiuzirar.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hvycrobg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2csiqmxzl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iqxcrekg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2saicuvnx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qhtvbgyf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wvtitjhl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pjcpinoe.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lrrtllnm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pbejiibd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2awpsejbg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2detoyywm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wujjvird.html


<!-- 参考信息 -->