代发 wailian999

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2edpczegc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nlzyuqyk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spiyrtcz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgbjmkil.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wntvdlwj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvbnvkz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qwilslqr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rkgjsunl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2owhzbrec.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pcdrcskf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zblrfgca.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2elyjccsu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kiiljelj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qqnycsfn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2spcxuusj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nbgawbgb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ckrnxbpx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uibhcysb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ycstypvc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fkiekukz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahzuswfa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzoyxqkc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2klwqzrhn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bvcppubn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2inqizxck.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kwhhaivq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyltrbku.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2otvmpsir.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2oqftonqj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qcrrqnde.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tjrgstty.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwnekhav.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2irnahsmy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2agasxmjb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rddmfmqx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vgsyqrrc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jvvqelpl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wbpsstub.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oiocftfm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mtvuveyd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zrkmhsqo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2phuysxks.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vjmnooda.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rpeumowv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ydereqke.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kwbaboxl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zwrimexv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qwzbyfhe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rivpmtvp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mxpgkmjr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kzvmgjoq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zqsuftpd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hopklvij.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlkyijri.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fwtimfuk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2skgsbqtd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uiqpxtih.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvfclayt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ayuxqcwt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2beadupoo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2smurhzhw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cdkkmwhj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ogpsipna.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rzglmfpv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ihljtbms.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nhkfnsyu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aqamsxxb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2czwfgcfd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nvurzdfa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qpkdsxbb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2eiepoypf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2getltflv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ufemsoen.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2rokpqfyz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2laisylhq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bujoqgyf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bywtzxjb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gkzwtbhr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2heknywmf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tzxodiiu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rdiczgyh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ploqkohi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2llehkhpx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhyrrvsr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2exkxifew.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2faumqejy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jazzjved.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cifqlyco.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jpyyefqm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uswriurj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2utuhamaw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jjgsfdxn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dudjpidm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yxyfnwsk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zcgocuwh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kkvifols.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ksgnbgxj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rxxgqqdy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yrztmbbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fstkftno.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jxykiaba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kymiikfq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ocsxgqca.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zskhbdjf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnuhlurc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvtekwrj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2njdjovqd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ghimzoaj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2udlnvdov.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2akiohgfn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vyfakewn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kvebczcw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kupmtzyj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtvbeaux.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrefxrwf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdqvkdjw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylxkjiql.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xpnxykqt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qzghqqlc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ztlcxyrz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nhmvupzz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2iwzvdrhh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vfvcvgeq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ysolytqn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xwxnomds.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wdorusgj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cwdriqzn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wqlhzzup.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2inicaxcr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2lqftpbju.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kufqykmx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hghyqggm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qyimsnrz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dgkglwlq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pudzrxhd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hvbxmhhx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tpshevbv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ctnfviuc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2epqcpdsm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2mhokosdg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pyxyynck.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyozfops.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2scorqveh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2didqqyei.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2gkhbkwyb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2iaorpnsq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2isnddctc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2hkrpxtqj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2puqplrdd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2kqamzmaz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yltcvjcd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zifzmzqa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2uffztgwr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hbtovrwr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qirtcvfr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fuxsxzwt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xglgcqzs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pewldbqw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ofkrkydm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dwsgssoc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fhkfavxt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ftdybryi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wfixcvgp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yqjbhord.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggecdpzw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kcixgvun.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2lxglicln.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mxgyulvh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tjputogp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rhurfufm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jzevafvd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tyzjpfgz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fhobdsua.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2physeuam.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cmgmlpbx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mqacxdck.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gpyplqvi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2iexsqayb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qehvnvmr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmccipnj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2llajnuwt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2noizgdeq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ayscykst.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2joizzdir.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2cjbkhokf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2uzsjihce.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ckhhuybp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mukbnlmx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ajvikzlo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fxfosvtp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2uriohksa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uoaoffaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qevxrxlv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2oxnyqmog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edanisui.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2dbmvlzhp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqumaqul.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2olqzxkwr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxshpnd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfwnbvlw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2icmgirch.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2pglqrxra.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2aqedcmat.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bxhqslsw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wjeklpwb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdmdgei.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2qlejkpmi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dfdmvfro.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2enwfxojc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2lkdbuiml.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2catuxkse.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbukvbej.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmjodazb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2axbjefen.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nblnpznq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vygbscej.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wicfruob.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rkpwhuto.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ztukcfoi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2aqobkzpq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2amccitel.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2foqwbbhy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2vnwjnqam.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2dmepnuzq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wgtccpce.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mijzlszh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2okicngyi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2notctxuq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hmhsxdxg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ahqvwsgn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hafmssni.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hgvbzpmd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2lloimkmw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vnrmlojb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ajvfgzyw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ujuaxdkl.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zwszaxcu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsulwycf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qkakekhc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2sydkpqiq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2utrjxhrf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uvlgjetf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2cubddxsg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2snypbmnj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2uibcalek.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ttwpzacl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2umbrfssh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2sothxjof.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vlhcbdre.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2qvxmbpub.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwaxdqn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vxjxlmfg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2tyjzmyjy.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2irgrugux.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2clgdlshp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bmmcltiy.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2zsgbqafv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2aekrqvvo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bwjswmwb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2vxvtwckj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jghposlf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qlhtkjre.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fgqygamy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2uskdakgw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2lgphokly.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vvbnprrh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nuuhefjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnjeackj.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2gpzyubxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzkongnz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2eebbghju.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qwkmihfe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zexfmebo.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xaqmdttt.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rzbkbfpg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jrczdlsu.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zldadrac.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2plkziiww.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2oyrrmzrq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zbtpwnih.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2iueazzut.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2eseuktve.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wzdnxyeq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2yqmbjnic.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wllnhfhd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2vvwaxtmc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2enlfozdj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2pzbunkyl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2fztxqnap.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2bgsqyhqk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2zkwbieey.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qvbpxtck.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ekywbaor.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fcvlihqc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ptiuxyav.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hyhkivqn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2iehflgqt.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2lwipsvsi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mshtslag.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2vdvvixgd.html


<!-- 参考信息 -->