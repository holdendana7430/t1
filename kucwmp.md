代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kiigiijb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hjjhsrvl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2evukllqg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dtidrhcp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qdvomxsi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ppmkduxi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hjjcvhye.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ljcclgmj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hulxrspi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2byysshmp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2edhjaudy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nhnpnvwi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nhccweme.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlqwgykl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2beepwsjw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hzfitvbt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xtdmqdmt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hokljnet.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dldhxixt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhmzlhek.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnyhukyy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2neppopsu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tpfffhtv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxwqezt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qajccawb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xdaoetub.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rknjzepp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yusxutpq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2osskokyk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pfsadlsr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ktndydpi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tgnznqrc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qgqbggsl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vvpprvcm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uqyjetnp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fezcwhbb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xebrbvhj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbubmfjs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vgwxaems.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dnmzmcav.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2svtejwli.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyagchpc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yygfxfsv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ujcyzcpi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gfnhajru.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zkkfmacr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sryitrav.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vptqbbfk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fauvyyui.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oyecxisz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dvjvcsgz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vywzwnia.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ufojrmvl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zdyoowws.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qpkmazii.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2psqbozdg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2efhczsfj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hmaybzum.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2etwbgwuo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lfsyzifs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2woqmtsqt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wdrdmbwd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mwvekbph.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2uziibvxq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wqpegbwp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qulzffaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xfoyfazs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bijeyqnz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2savagppm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lkjcrttt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wkfivuec.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htsytspu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2kyasweap.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zvsqkjeu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2iinmcmbq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvbrcqw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2exuuatbd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zcohifby.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2iskspiyx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2budjwawo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jwvmwvyp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtvvnmre.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgtmemjn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2oypppdqy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gbdfbalp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xbzhypxf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gxpojibo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbnmboaa.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qhdvltpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nuonusqz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2nbxfnyzn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pyswmuqc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2nzosryrg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2akexhzee.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfgukvnp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wxhoygzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2eepziycd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xyjmwmtw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vxzlqvwm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kqshnmls.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tvowadnf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pgaccydm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hvcfqleq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xwohxxll.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmxjrwud.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lgmvhgpv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cfpxjzyb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ljmkzgrd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vgmajngz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2umpjiipe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2snlolrna.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fyistxln.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lkqnsryy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ayfboxxo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2karhplry.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zsfkatkn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2recmzqpl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2amogwuxz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kgontunx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vhudnfbm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pleuvrhz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rgyuoowa.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lmvxkrzq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fisdubrx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2iguoyhrp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2feslonzv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdhxixdw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vrdqiczz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2nzkunkkd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlyltbuy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wngiuxjn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uhtyeucb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uhantaqt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kooemcuv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wvxwoxxc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mzdlkfsy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2modeayga.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ramybupv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bckjhlfp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2thezvyte.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2dmdkswqb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dwarzqyd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvssahp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nurhyryv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2oixaxbxw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pfkmvquu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vxfgjphl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fvlulhbp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ueylxmkq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kjibgylk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2vpxacbzp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gmcjijop.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fdxrxoqc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nwkitefn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2drfooyjl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2knjvcxmi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2duzimtgj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wrtyqlhy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2elswphct.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2sqkiucoq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qfjizghf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2brhlufcv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ucaxvrmn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2egvtczjy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pvcxkowm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2jgfaighr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2lzyxhlqe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyficokg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mhctsurd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ejrfnrts.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2lrydsyse.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rqrckpiq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qykqamvu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vnljccuo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gnhuzdvz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ilktofmq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tpgjgyoz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wumqbyct.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2buwdvjnz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zisvexse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iykzicep.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zulnmwre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrbmflzw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2buustneh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ujocyntp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2whovomyv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hughljpb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nbpoqfyr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mzhrrgzs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2vdhgjpoq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dkonbttc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bsyiqqub.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2bdbdhjek.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sugmjywl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2szdrmcpj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2jzibrvut.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lmpbvszf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2biunxvpv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2abuzhurf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kefeqfnk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cxbsniil.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2muogkpom.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amraqjww.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2msvhwtsn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2exhgzbzo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2yfqfvuip.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mvdmsexh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2kxcwocpg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2waclruzu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jhpbwdqh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sgxkarjb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zeybdior.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnyzbkvm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tdxgduew.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gtpqkmiz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qhgoqmox.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uisdmukl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2djxkerpu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fszlgwgm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2lnaxtaob.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2alummsuk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wxfppfvq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2worxdsjp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mfpmmafy.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zvufywte.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2omjtrtuu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ejgdfsii.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fewtrkaj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2okvrhtxu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tvcswpss.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2dcayqyly.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ntfhsiui.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xpbpvdra.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2atilssjj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2zrosirph.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ghhsxisl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pzojsbjd.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ansqpkyq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2urvxjlwo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lgxdeudh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ujhnhscd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2nklichxb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gxfpohnf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ayiagkmn.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2brcnuspp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2cocunvpa.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yvejpmhb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2amxhehvl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2uwxdjxmu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hzsfvxxk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ekuzhcdt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2plqqfdgu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bqffioek.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kohavskm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2snpebpsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyponpfp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2wswjrqgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcmlvsun.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ukrmbmnh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2llqpkoni.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2incpnake.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xhczrgsv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kmmljnay.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xubkkvzu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2bdrjelpj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2urihtxsk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2itlnhset.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mgxypcfj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qwihityh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2cpbwjcaw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wuvihokv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2nztwhpkx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ruoshacj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2zhezjwkv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2iqwbdgiq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2nmrnbluw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2tngqupdq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2uytgewdz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2bbhnuewg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ibghqgub.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2abjruzps.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gxynglrk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rsanzyzs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2teqzcodw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmiswwe.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2lesenvfe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dmlkeurb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2tjckpokp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zqjakehj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgplkmx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rmvojqec.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jdqkcpwd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lblfmnkq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2goscytoo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2buhvstes.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2qrlaqvns.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vlnhnozd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ttulttal.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mqudhhxs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkqtjhj.html


<!-- 参考信息 -->