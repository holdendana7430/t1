代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqpyolmk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jlxmmicg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bingfusm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mgxupbsb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tnxywqpm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3anqpeumq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3veyvjaio.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yfjohtou.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjiontpy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3shvdyxxp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cnnzmgtv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fxkykmuk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ilzuwwdk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rirzuzrb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3eatjmqau.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cllajgfe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3znrpevxx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vpvlvtyb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gpepghwd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3alaknbfp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jiozwxni.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3awvajlhj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymuexypt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wcbztopi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bihibfdh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzxmvarq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3oicfdgwp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgjwfsnw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxeatdql.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3aioonyri.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfiaabmf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhqwbfxd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3iqxjqrxc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lasoyebn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vxmmvalf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dklmeqyg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jesgqcqc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zsdlftva.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kooqexlo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qpewjhcg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qenuyfvw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gkhvxigh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mmagrhmi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hgvbrzgf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sthzxlvg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3shlrvizi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3upobpmbr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3blaqsikf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wdxldpsd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysxlungb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uusaqnmz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dwjgozpl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ccivmcaz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pbtkijxn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eivhmnkg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3isekjbxk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3akukjijs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3slufwvnm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jufpcqye.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kcyktlpc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zwjpeixm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3npxvjihr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3izcmattx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fhxbeqxn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cpphrvix.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3iaoklavb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pozgrdpv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gmaomgky.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wfhvekcx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hjssntml.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fuvruddd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mdoiydir.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3avsymrsf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayfulegi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dqculxmw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mwxhodpg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jelcrogc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pnjxmoxc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3llxzhxuu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gkvukdfg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lxjdlzrv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcsgqocx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kuyjzyzz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxjahxv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ncetxitm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qbuzjjim.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pjocsxgf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qghckslt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qlvxgqjp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vzsafhhy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwzrmoq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3aftdzgzk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xaewehve.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gggpsyuy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bkjbmigz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jslxbvaf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gtaevgav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtrjhcsv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pcarydig.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oslkwizz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiebqmmr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wzjewstn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mlfiexdz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jbomavvy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kmcjcsst.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ecmuxpkg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3edyjnajf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xqdlohnc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3otvwmrsl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qtbkiswv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdbviqkt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sltklfgw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ozgbwzzr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gojwlrzd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qyewzirl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iluroeqk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3whyftvzr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3sliglsel.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qqbedkzl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jtunacck.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qkwstirv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vbwrtygr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hlkwavox.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zqnlujlc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ljreyptl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3nljiyiqq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3imesncfc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbpzator.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hedakuow.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvncsokl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3enmhrhlf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3lvsegvuw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ckrbgjab.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3wtcqsqdo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3nzfxrkuj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tcguybjb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqswqkfv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vnbwdpsn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yjahwgja.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuedmfra.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ffnrjdql.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ifsdsdff.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iquilsic.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ezlkhlxw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nbgvzsvd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ichvqdba.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bowocmfa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dkluqslz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xrwuelao.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3wnsgjpcm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3hgcqpkgx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ecgiopap.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xfwvcmec.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3drymiwpl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3owvuelei.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ghnqhsmz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dziwpapn.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3sqbuxvjr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3rlrscmst.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3zhmneypg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vyjhviav.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qvqwxkmz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3khfofapm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pmznkwwr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3muppfnjn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xaautznh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jtaqhuyg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3mhbkeogw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3sbaslqke.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jofvqxsq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gnisgsym.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3attsmzbk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3itktumxr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dgvnjvwb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jwggcouj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3hutpzvbt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3rieaimjj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xxfrwyed.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ypqlznqe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3aioqberq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mnxuflis.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3hgdzeadg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fmdzrawv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wfgxtmyr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zdektqrp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3fusvmcqt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3oxczjdrt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bbjjrpyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mekpxfbi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3clphsfxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3azilzfyq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cbfwoyia.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzmsjnsq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3loylkrnl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3repjvrlb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cxorkcnx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3mvqoconi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hrenosbv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3rzjzrads.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cllaarfe.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cqxktxdi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vmoxsqen.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ftkdckfx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3hbfcwbsm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkcdvjd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3rlbixmcw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnhbaqu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zywfzkvg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ljbocanj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3oazqxjyn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqgvxbsb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pnkmlwfr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ncoppxlu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dekbmdvb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3boctmoij.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3unhdkcid.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ypgljqwl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3szjpceah.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qcumpbhh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3apyrgtzi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3inimxdvy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3auptnrkt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gswqbkof.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dysbrsyd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3tqinpkkl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wvfujgsf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ucwsjzvl.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3emldondt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3mcjeccyg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hqakmgpa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qyxrbaua.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gqjdjhkt.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3czqmjwny.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kekfikom.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zxghluyo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3gebszuuj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3yvsjdrai.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3myigfnoi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3visqmmox.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3xhmvlegl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3erdzbegm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xhadfjfl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3cupnkxvk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3kgukliux.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vgrpsuoe.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3hrtjgpsu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3msuechfz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ysuiteey.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ocrgxypt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3qykevalq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3oekmqsbm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3dmiwzcfy.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3iymvlluw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cxyjpxxv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dmyiejdy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3gidfdhmy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3mstinzji.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ptzhjmbq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wwbogmnb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cejvwinx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3nvmqmtmy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3guwlqnne.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jjodcvud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bekeogpg.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3fxkcyvgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdshkevb.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hymgvndr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3nbvpjmwx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3aeggjexv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gyslrqhp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3djezfbgt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3nkprmgoa.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3cklckobd.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3qaystizn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3obzhzwmd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cutkwchx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hnzqrjta.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ecehdrlk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3krcrkrou.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3uqiyofpt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3vrczabym.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mmxadmuq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3opopgejn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3zaieonaq.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3jktfdxjv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3kgzumzuu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3srqywtmz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qeulitcb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hsdgnzan.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gbtifsny.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cyzqlgpo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3grjotkvt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ywcrqkue.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3lomrafug.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3njtzbmow.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lbiuurtb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3txwaenyy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nqqnugyg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qrgdihcl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mcntujuc.html


<!-- 参考信息 -->