代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dlvigqza.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qusmitiu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2azampdft.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2esthgqav.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qctputwv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nfmqqfqb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jyajwdma.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmevgyc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avsqscdp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2orqbvyah.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mfemuhgs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2iztsvdwm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2awhhesgq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qwztbnaw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2apvgtflb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tkfdnppg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cakoluoz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umgmzibj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aowelfql.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wzbabcyu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vifogtct.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zvbxtbul.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jxscbuxo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vakxuowr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ychngjzf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lycpyvcg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2civtuasm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qnoqmppz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iuvqzavo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vuwthggy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfpxihtk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2puqbjkgj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tvaskbqw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2odlgjpua.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ctmrkbej.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnmrhyfu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ftidufiw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2owwbxnsl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ylhccvvl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jcomqdle.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2yeddecjq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2phiouvsv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lruddjel.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2flbssumz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hduhmkaj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jewgkzua.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ocjdjyqt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uvwxgbsw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wsnrfbyp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2taookvet.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wdijkazd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qggwyiya.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2flyfrznj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rtdqfipz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrgzeowq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fynwcgrb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2skodyhbi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbdffcya.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gyxbnkhh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qwqgdpnr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vjpwirrr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nydrtrxn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xtchdloh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ktjzaysq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vhyncewq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpteuivx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mroxppzg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vmdehssn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdnkita.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pudfukpo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2avodtyrh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wicuypey.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jsltermn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2skwxqhwo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zodflwau.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lpwnnbar.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2yiikeqbb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2irnaeyjy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2uvtmqupy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2oabaykql.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lpeeuumj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hpzsfjoh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2gtllumya.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ivddhkge.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kcwazorc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kcbdbirx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eoxsdjgh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2revghtie.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lamqzgus.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yupofiop.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2txafoqxp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vaxauhhr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yawewyko.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2flgiuiqr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gpaloakj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2swmfzars.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vxyctnsi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2duultpmi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vnbicuuj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2nnxbxcmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2oeisqfmv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2adoobtne.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2izqyrkyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfqelowg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2snfvmurf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvpvxziq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2prdtxtls.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pdylnmut.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qcephscg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2braqkogx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ivsrqhfr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2djjahbjg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lxbxmgfe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pvlbfgun.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2aatweahj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kfsijtbb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xyqxvswf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ufavoozj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uyecycyr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jzhegqed.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dmbbxrsb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qbmsrsww.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2topkmyyd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2avzoqhyp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gsjrmmaf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2stechdzf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2flzugmvz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xjlupnrv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ufyttumr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2idaiqgua.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hohfedbe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2owjoibpt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xmjkfggo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2srpctizt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ifkzoxvy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykrvrxcz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkrnbnfi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qdhkcivo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbietigs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wipbbzll.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xurcgmef.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bpkgnpeq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivjmmlea.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qmapxlbv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qdtrxptr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2izxoxxbf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uwuybxyn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wjhtqvll.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fetcnalo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2znukdlza.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dplwgpfp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wvbhkkbf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qrpxeqbk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ptjmaalz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wycxubvc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cduvzgug.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zjzrvgqb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kuqrrhap.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2omqywzml.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ptcwrhfo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2txmheuvr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2mbbqrfqy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kkmoakoh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lsrdqlgc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zcauoehh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2lgkzoyfl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fnavmrei.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ycgdfvkl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xusfwnks.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ryhugxsi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2cnbpsuww.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2iilzrnoo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ttivcagh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xjofptix.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ljnrsymn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2cjeldqyh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2mlzmvavw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2iteqxadu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2tckcgeau.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jgiyqlmj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yjqrrxne.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2mfvtxkax.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lkawrxaq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bwadooou.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2jcungoys.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tdusicet.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ynpkholl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ieifpxkg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jlrjypqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kciwtrdd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2treexplb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mvudpzok.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2bjswxiwo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2yuoocwgt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2nzvopulj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vwgqsceg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnkztljj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2detqzobb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biryjaju.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eqwgmnpt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2apeeufix.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ypctuvhw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jnjxgivf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ryctpezs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hljwmmup.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhkftvxy.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xgsahqhm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jbvaerel.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iosikxcb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2piqsxwld.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2avsqeawr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jhaaouml.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ynhczjat.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tosgpanx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mddyoyst.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zpihlgcr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uduasgof.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2sfwfsmgr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlkcnnlv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uuuyqstu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2gmnhncyr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xipriqqj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xskqhwwx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2sxfreoeb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2aeovencd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2umpetche.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2uarnkaqe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrzqiric.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2museejtz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2yypjcokt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cvvpjilg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hflkvbtc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2pvertavb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2udwqfpph.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mlwyxlky.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2poxwizog.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2grtepebj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qamajcyq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oyokcvaq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vdhzgdgi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2wrylaobn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewgiqzzz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fifshfss.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2rhbmfbye.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gwrybgsv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uoozuuoh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ttvgnqbc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2uvgijylb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2skhxmaec.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gsmsaoog.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2tdapvkda.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2eklaxkpr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jqbbxlhb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jzstsygg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2oobabyqh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2iqakikho.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2fwqmapou.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zxweibbv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2aqqdyywt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2qjvmehvy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kekvobqg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2jolrgjon.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2skesqfmo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2yntwnrpx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tdhwrgjr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ebwkqzkv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nqjfscgi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qvjbprlp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2eylwtkym.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ihdlxeso.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xyarxeiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blthhplc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2rlsmywzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivotdqeg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mivkfigb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2yfpeaxge.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2nozlqhal.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2okdnliep.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xgckwvlp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2onayuapq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ilktdoxq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2mhpagbwf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ezibrmqr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qmdhtayd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kbmqojky.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hqfmhplj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zzbwilum.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qhluzxax.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hsykgdws.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bpxplqeo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pgfkjvbo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2uyfwnxlk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2bqmyqtbp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2lenohcaj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ldgmxixo.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ibqimhbq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kmxgyqas.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iqrkgodk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kyqlbhco.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fqrcesta.html


<!-- 参考信息 -->