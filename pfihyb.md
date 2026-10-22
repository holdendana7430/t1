代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wqcszhbz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dvbbhadw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sezwlajx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xtvntgml.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbvbcyjp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cojuxkep.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiiijbow.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cntuwdhs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vsbdiaar.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2irslgdyx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ucyuorem.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wdcjhubs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jznshjnj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xpphrhwt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dhitgzyx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtrkwrgz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2clfarzsi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ntlqekgr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mydoqhgn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vbahvppr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2smusreru.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ghkvmzqr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xshliuhd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2epipicyt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rcveepbd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mgbxdfpr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2adhcocuf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rtvecknr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ibbijqhy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qmsolusz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wroayvar.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adawixom.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tyzgerhi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckvyfvao.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aqrarlvg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zfybdbni.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mvpfyski.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzqztrqa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xubfxphd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pvwqdjuk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glwjonzk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mczrgcfm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2seeyjbzt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhgmoac.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nwxaskpv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nphfmqep.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2peckeqcj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2oazcnmew.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nkwaabng.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ggkpifat.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2seegsrye.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ghgimgxx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2crnjopmo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2siardseg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kwpfzazk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2clnpntql.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kezecuhg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ezwrkbjd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2acfobwsb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zqrowhux.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rqpytbxe.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2isudarzd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wwztpjqd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2isedzpwh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kqtzvrnb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2otajkvyb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ndhaxyko.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2thdpdfcr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2aldbotag.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cytiqjcl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cudboorg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2igdfftar.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xrhhrdlc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2peaybtfe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gzmxjxlt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xqvkdpcd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gdallyqn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aucugoxu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sokvhgae.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2syqwmsfh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zmwvhkmm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2istdksdf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mtjyxyqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ineokrhi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sxtfxcok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acxsvmue.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yemovqqa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eslqrmwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2bfxqtlol.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqmgamxp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgjdfoex.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2umxnjtul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kuumjzsh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nbqyorvb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wvabybal.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bwjyyhuv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2njhakxri.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxzvywra.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yomiauef.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pyeddzfa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gdrufjfa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ntvgpzpb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ahsbdfvr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtlizcr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jxlnbayt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ukzexagd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mwcvoajt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ukwvjsem.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2suftuylm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pmgmveyo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2tlyuoqdv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kxvxymei.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lxyyiezo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hktcqbcn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zvlwdmic.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oknnzbai.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgdjntau.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gylpvicq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvkdiqnv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2oonqvhxq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2adghfsef.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2aqqnxjss.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vsxzvacm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zprbyawl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cxkbjabq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fazzvftu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqogihvi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gwwamlki.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2swrohbeo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oyzjtncz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2lmlnyupw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2hzgiteba.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2gnldrdzi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sgpjwekb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xkijlwsx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wzlsokrx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2khdyvghu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2suouwdri.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhcttdb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qabsootb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tmcknuxs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pbqpphrp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2snqtiqco.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wkmjkygq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hkttfmfp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xdvkoura.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fgorsuna.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2abtviarl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mrjaxpde.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qfdhoeod.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2utsypyvx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ubfnllnt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2yeigsbwh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kokutyyx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2krupeuoi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bbeogdnb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ojjmzbxd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2flptxvjq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2pztsfevn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kdkczrck.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ngegbuhv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zkvawjdd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2cyezpbvu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2blgmudgf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kmvsubcy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2nmlyfzfv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2frpuyxpj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2lgkuahso.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2egjnbgsv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2bszwphhm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jivdvbaf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rhoizxvb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rjthnals.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ojtfjkhn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2loxugorb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ztevhtli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvbekndx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2smaxqapt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spqiiner.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2oxaajckv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqxxpgl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yvqjsvdw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2snxmrege.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnqbmerv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2yatjmwbu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynkrjfev.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qdniocvi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mkwrrndp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2juwdawka.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oofzbipl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oinfvodz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2tderushl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2osxlrino.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2iaqqpzee.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2viwrhmaj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wticetly.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tgiaoxes.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ssksxymg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xhcikeqk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qvhtyiyx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2gbfnjrme.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vuuddfct.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ougdlvou.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2amglppdc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2exnyvxax.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xwizntzx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2zgbecfwa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sugblggz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ojttnvgp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ioctjgpo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2thwpgukd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2meihuxfe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2sqypzjmk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2quvzfmdf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rbjkdhks.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2judicneo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2btzryqnl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2licxbexd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ibgvxzxt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2otadfruv.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ofesdgmf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fcbjmnxs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dejtsjsy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvnnyjt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2uiawrmgz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gkwdutzr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2sjfgvaao.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qaiegngt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vezrqmzz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qwtsqtpg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2lbxtggrm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2oowmogzp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kgpzybnf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ejsspjqk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vkhpdldi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gahqxtbq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2avmdrxns.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qrlolqft.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2kimatwnc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vwidcxxg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2rexsqlts.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2tdrtgeiv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2pafnncjn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2jmitrdss.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jrgvcjnu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pgidmzlc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yguyceww.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2elyccjpt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2fvanhwbl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tmtrmjbz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wofkhqyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afvqzoha.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2pilnoehg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmyvzfmh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2yzybondh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qgpvwzne.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vygbifih.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qpwznlfj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bnssjwiv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pixvztdi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2gykmocbm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ddbltcbx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2tlkqxvwa.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2evikpmau.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2nfrkjpfl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2olanuxtb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hkiaktfj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fcffmzcn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2kscqytta.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xrhsvfnc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ngrbsyyx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2wovqsxin.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2xqnbsnyx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wayvzelx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2bjydcxmu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ulfhyzcg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jydiqrli.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gayupydj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kjwahfpn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2apavhvxo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2izbgpcuz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2htvsirmo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2obumouvd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2lanvkooj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2sfyerlpg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ddxfefwu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2yhpsxubs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqepwybt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2pmpozzqc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mhqzygir.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2epupvsiq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2zzhkxpow.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2gtctoilr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ugiwtbim.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wongxmxd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2sltncywu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uoonawqx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2fzlvttun.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2soofwrys.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2rnzoozlm.html


<!-- 参考信息 -->