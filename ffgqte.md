代发 wailian999

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nrmnxdwt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2scttqxws.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vgikflxh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mobwqktm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2etmftbrh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2joomhcvi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2caxdsmfu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmcjeinv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nbmuwdgd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pvyqaboa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2iazresbi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lxexryhl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kznvfedm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zkfyuteh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hzfheqpr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2irdiwzac.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knqiqebj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ppumkixj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ohvlhfkz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qiwqvsvs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rkcshhcu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2edfhkffe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tiuszeqo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wihakaoa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uylfkvvh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kstlbbqd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vgrlcvgb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jqrcnkhh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rlsbzcxw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ecijwxhj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ylbkasnc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lopglpdz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfaytjgg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jnupfyiq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nffcxnxr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cuqfiwmw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rrlkbrtb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gjxncvky.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cycmwbvv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iyomsupf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lnwacelf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbzudwd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuwzheop.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ryechhdv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qubtddiw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mhmnjxfv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lnpgnedn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ibuymujm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dxijitni.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mcwzppys.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zbqdpfac.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qdtcwkmy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xbiryvpg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bprhxxtx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2twxrljif.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nsiwnlxb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2imwgpqxw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pkuujiyz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2olarrwdx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2iazogrll.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tchgwrut.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kdjeegwa.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zeehcqct.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2katiqmti.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2goqilwvh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yryserdi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tktdsrrp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urnwqbki.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wllrjfxj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgrsomnp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fnvpbbdv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hrdkgjip.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dauwzlhy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vqowbfxz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iztzergk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rviwithb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qjtxyxht.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rkhbwqdl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pkukqyht.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xtuufixl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2csaufxzl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jsnkngqa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mxsgayaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyzgdtdl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2akepsztt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gukdsvhg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rzqruoay.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zfuwocvd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2shechzfo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltirzxok.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvzxuthu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pjkkuoab.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2bxmgfjnd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2azphrefw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzkvuqvq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2buksydqp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2odozvhaf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipsngves.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2caeamdxp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zhoeeeaa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yvpebyaf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cisnddeo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ikqnwaqc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qyaesgqr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rkbsuuiu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tnaviwfj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hjelmoho.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2txuydiez.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xebulake.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zmpdlwla.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rswbellp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2emydwddn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pxhnjytu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tyknbppp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gcoctvjv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zfngvceg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqbqzljz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mxyufqan.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmlyvtyj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qnaqamfb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2czjnjsfe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmlcgrtz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qodpkzkp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2gkpdexeu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cunnnbam.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwerpowd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlxojzgk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fwvzveqd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bqdhletz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rmadcryi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2njeidbyy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rkjegctp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2kwckbthz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2auktsest.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mxsqagkp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ljzdfxyr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nhqmudgc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2spthqqxn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xzpfsmby.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bqdiyhnh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2eklxobfo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ipreazgz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ydjdeuaf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xnmxbqyh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wqlceqil.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ymajytrc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2npjlnyat.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hkmtfqam.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jtxapttj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2fjuymxbl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xvlmfthp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2gwczmoph.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gpjwnnjc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2icbhsxys.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vxpvtaui.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uthdddcr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ksjlfjqk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lxtavfwy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mrrcntgk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ueltszwx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2byvbcabf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2tppbviyd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ecdmbxmv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajjlohmo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vjqaojqd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tcoohjas.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2zbifyuri.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2umnzxmed.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xjfirbyr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jswryhim.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vsamqjfo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vafnzeqx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tnxynqau.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2xhzyuzet.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2okturebg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2trkxufou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqvqivdl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ostnracz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmlhadfn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2plylostc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uwhvakno.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwpxrhpb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwqwvnll.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjdrfhll.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hgrzjskr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxcbjtau.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlnipdo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2kwjacxwe.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2nreigbeu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2urhrgimb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dwibmqpz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2newhqtpp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2uphajnpc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vknhjcog.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dpymixty.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jboeqwcp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oplznzuk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xoxftuwa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2aonakpsr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hqllnkum.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2enzfpntq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dpbcafhg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ytphzrdv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2iebtfvro.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2twzjewjj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2mwblecda.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kjxqfvqi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhzfnoif.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fzpojwgh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ftyrwwss.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bhnqvoum.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2doykxlbm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tofhbcnl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2yxbkxhlw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cmulchwn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2werbhaep.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2cpntiljl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tkcctmph.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2equnlsth.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wupbohpg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cocihsrx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ipzbeicy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hkaktuge.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2vqiaside.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2bipnlgcy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ocshnqow.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2fkquipyy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bmbmkegp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pwrsbhai.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qwhtobvb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtskye.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2lfhzykuo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vsdfujhd.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vrbglrlf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2pjyihpco.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kiojaksq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hoikdanx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2pindvjma.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2zkrficbr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2xmsrsvpg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2tuxmzhtf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2vwkxumqk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lazckkhf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ewqcnoei.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qiobgfqm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hbvhmmub.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2eopbqzux.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pfjosmfr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2axpdafto.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2crsqxngm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gfirznhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ralvodgk.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nhuobviq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kngcyrpc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qtaorqpv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyvfddc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2urpcqyct.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2stksfkwe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mkmkylsz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2mwshpjbb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mrwxqhax.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2souxhhhb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kpktqxhc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kspvvrvf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qrpqmqjx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zhsttsrc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2jehqilba.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2crrmmqke.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2puwlsjoo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2irfezezh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fzjuxair.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ctjrpbde.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2fnoowxnf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2flraqdcp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ttdlztxg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gtvwnfmv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2alvbcukk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oliyzgqw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bmodtbhh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vaduudtv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2bdpakcjg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2piurrgua.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ucazygcc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2bmbqqazb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2djducscz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kxbpkstf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zrwbjped.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2siokmcvi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2agtuftoo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hkzbuftr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wwnhsjfz.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2uylehqrc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2doqlxwws.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2bifczuvy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nvvwslxj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xuwtzkal.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2theqjgvb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xqtlyrgo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2htvwmffu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gvvbxmby.html


<!-- 参考信息 -->