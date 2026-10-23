代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3teljjptr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ievryghz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qypogymm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3aducpojg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lyqbricj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lxqatusi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eyfhiarw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qdyrafdi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jotogqia.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ktmxbtxg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bxarcpjr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3keysebnb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rtdfcvqj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zecndopj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3exiuyqog.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3borglaav.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qgqiceoz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kztotidi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcxssnss.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nnttfmnc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tekmbjif.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hhdpzpwt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hoxcbeyl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jadyxyzp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxiedcpx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3huxlblvg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmetgddd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3buzfrkbh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3paihfrcq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3srbjobrw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aeilhcky.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3whensjov.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ytbkrwsz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hcdkokog.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rvbzjkql.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3exlblmsh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3akoctqme.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fzthbwmd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3hqoufayu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzwsrzhv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ywukuzqj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfurjucx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sgapxtsn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zfcatrdx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vqpxnavr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsiejeou.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uaikbxcu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pqjexvdm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hpdflfce.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upvfpmtk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sugebest.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3daullxac.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jelemgdv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rxirvqeb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dhezmksb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tpxsgvvw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xhdvdevz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kgevhrkg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3byepqhmy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xvykiwnt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zfnqmdix.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3booclrqo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3imgprrth.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fmwvzrez.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kgwbutak.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3obicexuo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3skttwpfc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vwsqoepb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bjazaptf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkxzcbbw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bxlrfhae.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oghkztpk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ojuccajq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3irilygan.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sktoxpdo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfpxpdl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mvfemvhg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3atzphnvt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3znumrglc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3exjzkukr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wmtxdpkd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rvqevjjj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qpknvnyi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rxwwhyui.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wpominkc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xshlwbhk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pjfaevgl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fdmcyzxv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gmumirqa.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dwqklmej.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3odtokvgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txlzrssi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cjsrhscs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzkyrscq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uyyglrwy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ijundbba.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcairtfn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbdcuxxv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzcymb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jblletrb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yrhtseva.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ebnxikpf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kxetmgqn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ulbxnicy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3txbxjhpf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ridteghu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qjsicnry.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cumiarkn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbebecce.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zuvchdpq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rxeeypgs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ysztrmxr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3obogriva.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ydgdjxxg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rwgildhd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pdhajxrb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3auornzix.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jorklndx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zvnicowy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zvepbksb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ltztwuwv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3dsyfrwpy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fblnfncp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngrddamv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3koekvkpj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fkgspmia.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3piwjfghb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ynvxfska.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3poltdsva.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3azzgsgyh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mbfjdbug.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rcpathix.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cyoddxfj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3luzvhset.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3macjhkli.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqoipwld.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jpmawzsq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3pxughmiw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arrlucln.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wmfouigj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3aslfoeni.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3iivzhdas.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ukjkbtfl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tzlsbblv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xgonrgbd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3uglgtdou.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ddpjiqaw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tglybtwj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3kpviyngk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tdavapiy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3transkpx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qkzdubru.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rdromvfn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jgqjktup.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qwlfwssb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pdbsulcs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hyzluznp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lfkhfdpb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wyopypvj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3extmgoop.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hdwqxhhw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3svlqespe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pxhmpiyr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3jzrmfnod.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xnpucahh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jsnvyglu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zhscluad.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jbtczomn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3epqimsid.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3jlgtekih.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovofbdzo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsidaaot.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bvbscdya.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nqlusovc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vclnfibm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3lbgcwloe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zhayvqlc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3oqpjygvu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yrhcjqwi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lgronipk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3kkmexlag.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ftaorpyp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3wpjrcyfu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eottghuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skgruxhf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zdwqcgna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzhnwque.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xqfykgol.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpihkeu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ebjfhywl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwvixfq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yzvzgiww.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3aslofpzb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfxwdteu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3splkkbgf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3scjqzcaz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ftypwxnm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzrlfygm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ogpdbgsd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3uaydcmle.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3pxhxztjw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3erctcngu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3khdwhqfb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcwrccv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rkjmhbpi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3okekesik.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3fbzwgiuk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3chcjvzxu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3upvhvkny.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ifqkhvcc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gspcnrfv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3pojprqar.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wpkhgjwq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3lfzvlxaa.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3aqzvpuqi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dbbratfh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tipbhaio.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cickwbxw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xjngmtko.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3quncvayc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3jvacmnxj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jvomnrlh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fbvrhqiz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wtsmbnbw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqrhxtvr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ahtjovkq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3urqlysyo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aiguckdk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ufvmzqhz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3viouqcga.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wilkuyvf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3rthdgxai.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3mxpykjmo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sirjwzgu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ekkwfsrj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zjjdxaqq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xgqxjbfy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bfhqlxfd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3sgmfbeud.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3rytycffq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gbgrnebh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3rojeurzs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rkjltdpl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kbnnjlhk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zabvvotv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3xihvbafg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3vmsxwcyi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3bvoivlcx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tdfoguxy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3gywclwiw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3fjwjqjdq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rarbohrq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qcscxxvu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3godcetbh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pzxulcdl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3plruasig.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3bzmhqyrr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3fkltnjoc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qxvaekzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzvvnpdd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3banwokux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baqxrqjc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ieorrqow.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3uojnffpe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ebbgjmua.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zboppcus.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3inikzzms.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3xfkzmtrq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3aonmqkkx.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3htcvvxpu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3vschzrbv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3icpnqgxd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wvihdlxc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3khzonfoi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3gwiosyij.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vuhxemuz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3edmrhoih.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3xzllvlax.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3owekvzrt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3vnjzarzt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ygtzstrs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3nmmooijo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3pjbvrtqm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jpghfncz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yvfxknlb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rhlnwzwv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hgneiyti.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vlroszog.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xwuodxdq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3tkxuufqb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3srhwylzt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3newkpjub.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ckvbsupx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mszyftat.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3kqxdwaeb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ankevjcc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wwcjkyiw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3yazrrfcj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3uqwmvvhb.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3huxoitbw.html


<!-- 参考信息 -->