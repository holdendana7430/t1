代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wvahtpfv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hedbcsrn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mubiaujw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3iysyrpce.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3drvxigzy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ckxvnglf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiuqqpwd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kswhajqd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wwrkdmuw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cfrvstdk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxlihbnd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mboebuxn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ebksyvmn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzlrmfmx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rqmzmtkh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qjnvkwxh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqpfwjkg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hiallmnx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3psujjsrn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rnwxlklf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dlpvlzgj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wdamonvf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ixzrmttp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rpahxpcy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3owrdoqds.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vugyczmn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fimsxsvt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wbagyjtp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3trywjqhm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3deoimcym.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rarmavmv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvdgcyhf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhndceqc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrmywlaw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bmcoegnz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kqqutodv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mtomvdco.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhrdkxiv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fuekpowb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rjbxyizw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hypedudp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3czycmcsu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3aeeunhva.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pptwznem.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xeztlnlz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qaxplemr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qflxbrxz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dhklcxkv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nnyqzjdh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ewcgpstj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nwlugyeb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eysgcjlw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jdnnjjjo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zhrwvimh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcchpdw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mgcvxsdf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cubrddcm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mspwiflg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zizeqbwt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3golxwlnj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qpsmhdzg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vguggkwm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qqtaqmzt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wtlzuonn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bpmtpnkm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cobgfwny.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rbyvcxxy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ibqxspor.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ddrghaub.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hvlbirqh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dfxoxxpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ufdxcdft.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qkllsljj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vphhgvuu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yrzmywso.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3eesrniwh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ghfjgjdn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ufkjwwvv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wxsymugl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bupbnwoy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bdsibwsa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nfsflbcr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3isxgwwzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdrhhqzi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wnuzwibz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fppbchxy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nneyhiiw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yjbmweib.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkiuahmq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yhhtbvjr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ofekddqd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kggavhob.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ckihtlml.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ciiptuae.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jimocxvq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bfwmupib.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3otbcnsyq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xdyguzoi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqdmpnzv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hhiqjkzl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdzjxwiw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gqetkptg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3bjoevfdp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3miwnkwkl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ievfowxm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bbladcok.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gprrgwmj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qgkncvff.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ftssjgwz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tnctmbca.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzseqf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uraxturn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jqwrrnwo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rpnfvbyq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dczyvihj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyxinzcs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3igzvumni.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldtdwjfz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fvqlxear.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3chudvmis.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3hrfwmbin.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3eetsqmgx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cbvohfiy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3tlweesou.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vmvjjfek.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wcfzzxwy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dvfkwato.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ljikfirn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ihpzqzio.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ugcyzvry.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmevmgkh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kliqvpwp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qooismld.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3elwucesx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fylidqxf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uwikuoqp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3cjvwadjs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cdsksjqu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gzqipmsu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3cipbewjw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3eaookiep.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vjinqtrd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ynlzpljy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vadvhgss.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oqxxjwxj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3oqshfcyk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3cjovmfcs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3eheyuxul.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uhouaahe.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hchmbxmp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3plogjdcy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3zfwrayok.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3fbswmufe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3etvhtvhe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ydxsxoms.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3nvdqlcmr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kqdzojkk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3lwhsuavx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vdmqljom.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zzaftihn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vowtpwtc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3guzdokxp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xneahbqk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3lmygptli.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gatnjzyw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3pljkfjzj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3hwygbuwd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3clevvqgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3celdbsna.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ywahkcpl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nfawwmbm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bzmvmhjn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3flvxhkhv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ockgjvpm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3tbkjxcqt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ntwroyit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjeszadq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rrypnmqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxypgzjx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3dcyetich.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zfmxpboq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rxxhojjn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zrdbyvyn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3budmedur.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3lhehhiba.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3dzmrcuyt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wpsfqkrd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3npqowktn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3arlokitd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3osstqfbx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3awjcdbrl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3gdlrwkwm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fnsabqpq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fxyjydbb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hazoneyf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hqlcnpvx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3beeptrgl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hdnrawuf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3itodovqc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nufldbbd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qlqnzskm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kcqtakpr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jyxspkcf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3tewemamq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3gqgihygo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ichsnfhf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3gfytddle.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ygurkxjx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oudbdbbu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jfvmzwlg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3wncrtqbc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fklxxmcf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lcsawwgh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dbrkmvbp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3orlubhhw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ujuvhwkh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3txuuqzpm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nuxwcujn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bdjqlcbb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vbmpyahy.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3blfvdugg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kftpgtra.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdweohp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xzvpceqk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3bitvthiz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zjrbsrtq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3iptcflhx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3twtsjwiu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ghfhhgqu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3viovfdtz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3eguvmwvc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3suxpatti.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3enbikhno.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ocbmmlnf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wwwhoceh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xmrogqoa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zpbbmefa.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3glivmofg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3wyytuqjw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3hktzlarv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ssiztnoa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3cxgdgihz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xtftrhrj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3cxxeslxx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jhljkpcn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jzzwfqdu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lbifxeys.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3wrusbeaj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3bdlesvst.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3bazidpma.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zebmpnwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ihnuamri.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qeqpdtmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxrtfgun.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3gezbrfqu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3rvxwpnbw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xnpvwiex.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3iycxnmel.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3shlamxns.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3skdplvpz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3aqjjfued.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jxjtbtir.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3rfgpiixm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gwnrzzjm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3puhvesjg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3koaqwvcd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjrthvq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ininntuu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3frufifsu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3iindahbn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zwhfnbpe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3vtdikdub.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3wwihkvfm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vgtgkjza.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3cekowrmt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qcvtbksp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fgbibtou.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3reipomrd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wsfdltki.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkklfdy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3upfrvveg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3lzxrjebs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gnxkxvsh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3idngvllk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnlqath.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3eeiiocfg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3miestsog.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3esepwmlq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3wknurlqo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ppheqvit.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3qplenzle.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3avfobnfo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3kfajoelh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lvhjngso.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ktbchxhn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tamzksfh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfozqvv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3gvywluwq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3agzrgkqw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3xbmsihkk.html


<!-- 参考信息 -->