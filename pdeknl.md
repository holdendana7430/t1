代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ezddwkqy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2upzbpnrx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rynkvjbe.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2edrqzpgb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nzggyuio.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bluurubw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gpnrdtuf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2geoqyhix.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrkxygwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hrlmxtxc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjuqhsql.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wjnqwkns.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2orxadqli.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uysshjnv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmvkjqrg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbueaipc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovgjrjqb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ewzqvkil.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nmuerghv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvpaifnm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dtmtpsmr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2akyxiqgb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tffpuufe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gigvbzrl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hlgilexb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jdvtdeuu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rjnpjpeo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hxpbmdhm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2slcbnrdd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pdmeixpt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dbecksuc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rfdgcgzo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctuclsbz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhbfwgcy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wzrxuacr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2sbwfsogt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zwietuve.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixnhymzy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gneduuqb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xmydtchf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mmgpthsy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgisxbst.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rgebovfn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzreqxdc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dqvoyelv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2afmlvwpj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qypuglpf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ieqexqas.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rrtktjoq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2obnlwhjy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sxahazcj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dtizbrvt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nwtvsebf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qopswqvv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2giradyrd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rxsuxhtg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xfwljfov.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2phscjvlw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2oykxutob.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzoggozw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpjtteyd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftdizzzp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvbyvtrc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2blagwpqs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lbvhaqlg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fubnmcan.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2slgmtfio.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tgxxzrgn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewihahos.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sdgmbhvb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gslxtiwt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbtpukfn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qeucclxm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lrgmjyfx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oabkxgxw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eceracrt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vufkpudr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cswtyigu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kwxpdxnr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vwhtyfpt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2evitacaw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2adsnkjck.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rxpfpwpe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mapeyqei.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hicfsrbf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2fdbeonmc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2rvqpqjqi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ehuqrwll.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xhmwvger.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbnsxnzv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xmobujpg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hlhjakps.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ahiyqctt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qvgiiwxz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2padqzexv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2uozzhluu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zhxesauf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bqbsjeck.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2crrjyjbe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ggjvhfaw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qnoasoma.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2acxhcmth.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qclxjiqh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ynwjnssh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bwfpzbhu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dyxjqnyr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tdduuzgt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2waytsxdr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2nntwabdu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jgcscrio.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2shmmzqyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqgdztol.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rxdgylnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aulrdyep.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2rstrlnts.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfhaobx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uaceipqc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2apvensnn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkltypnx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewlvvgjw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zbfxrxtt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vrjluxbi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljvumccf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tvlbwqlm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2msfynebd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2izprrtwr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdecvwks.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ckfvarsl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ayokpeok.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2npowjrhu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ajodvdrm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqeaivg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2svqafglc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zxjdrehh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yszkmrkf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mvferrzg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vikfrbar.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2riseniyi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wcoodsqw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yancnccc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffqeuqji.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bqssiheb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tdsdyeig.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuydoetn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywlleawn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwhgerht.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wddmiump.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gvpinljy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yipbscje.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdkamfab.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jkbchnbx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ngeanetl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hcvbkyrk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wvlqjkpy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2goafuicu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylupjzve.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2avfozrfp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2btbcgtba.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmqwfoct.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bogfxwes.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2zwyhhqsr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2voyzriqc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2svwrpxec.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2goepxzfy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2oinohiyf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2okssfmps.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wuwrdxvm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mjziuoqh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2bfaraxae.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ffqgwtzg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lsdfrewn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vfvlhcbp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aeqrdrpc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2chnenumi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gcxvnhri.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zngmczwg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dpzcrqji.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zqjdclpe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dattvwnt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2vpbcxfmi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2djyklole.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cxctmopz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2crpdtwhu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2yyptllqa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zsxlqquz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gupnyycf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2izbahcmb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zwucqagi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qnkocdtz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rfuvlneo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bjxtueet.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2cawyahvf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2phdmumpk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zuemlphd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2mepqqjxy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2dzhcadmc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2aehfgfeh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gzksgsvi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ploegrud.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2umxktxfi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2wbiuakrq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2seqydkca.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mrkgyigh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qasvhoxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtflptpg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ukbenpgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcccciqa.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ewpgoyve.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ezuqxnud.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yfudedjc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stzvwlvv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zebauwke.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2trisidqz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwcnqaao.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nylbkjhb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2spfvammh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lcomrugt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yngdhlqy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bvhhhqhd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hjoockmz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2upsmedqa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlapbtbf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rpoepynn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bquuxboa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzssyvrl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ivpdphie.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jumfhyqf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2svxylwoq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vmiqejym.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2duklbhje.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ycduuexy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2lgpkjymq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tnkzuarq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2tyranqmq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2fnrckgxh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vjsuunsf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xomccdpg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bufbskjf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hhdjxxgt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ahqycmwi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gblqgbjs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jwdimzsv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2csynshpn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2cvipzbse.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2lmrazkjy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nnouoott.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zenuqxnn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2emchxppu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gbzselbi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rexcxjet.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ewggwqbn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jhrfjysa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zwnraouc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ovmusqyl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2flamhsvg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2staccfgf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sjpnzhgn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2edcoafia.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2bxqbdrvg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2zthruajc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gzpfgjso.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vduhujak.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2oawlyvov.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bspjgqwv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2twtldvjt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2urtnmqlk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tyxmkgfn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2wtxfkytk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2vishtdzb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2mghvwryq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lzblvopo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ewpapsgx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2nputngdd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2tvdbnxrx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gmpcwxnu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ckjjdpgr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2zqsxjkfw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2xknkibdc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lviljllh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nervhzve.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ljuaovbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usdyanly.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2auamsuoo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dtdytjeo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tsqdsbny.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2waqqvsld.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sfywuopq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qgyicjbo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ysulnaby.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2xvmivset.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2opiitbtg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jfbcbaih.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dokcfdvn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gyriberk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2tgedlizy.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vomphrzp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2rbuavmjg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2gyzixbyh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ognlzqee.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2tuukninu.html


<!-- 参考信息 -->