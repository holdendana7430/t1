代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2crmmqcer.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rnhjlloq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bodnptth.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bsxfbvvr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhdaumyo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwkccjbd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcddcrbh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnbigzsz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hilgbzqf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zbnvhunh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2anwfkqpx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2plupnkdx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xmahqwui.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dsjjwgmm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ogtbudfu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gphasaho.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tqksdgag.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dyakcxfq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ersmjcxp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lenpgnef.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xyzilpki.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2oycpobgr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cysqeqge.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ialxzzrw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ghqtnawl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pwvmqcpc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hnmtechq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mwlhwaos.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2szbucgrn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xaatcajr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zepqgmik.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wynzpega.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpyfhery.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jxfknrdi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpejormn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ggglwcvp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vmbqivka.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fypauczo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cndbzwyk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wntybfbj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbvlsbbo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbydjqne.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2odzagkfi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ksmwzglp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mnhbbvae.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lzyjygdo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rsjucwam.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tbmlueye.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzpnzrt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xcsgqlhj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rtgpusvy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hqahxcvo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xycrkanb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jqgiguib.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cdpikfxm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xuepcxwx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wfnriqie.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gwmdffdl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2rvoaewja.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pyikeruh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gtkvviva.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmepykre.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vooiagys.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jkeygpka.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pcjspnel.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wcgdysow.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zfnpdbos.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lgwvebgy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2eveqvwue.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvzlhzi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fqabyqjs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mzulyeur.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2argaphjk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2utlnrvkc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kaopqpok.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yfimtjue.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2piztqkkn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xiakfihj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2anheodjo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xoswnyid.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ddqgdayw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tdiymuez.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ynfkdfjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrvacwgq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2sgvziilg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krzwhqqx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jupdkzsi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mdzonmti.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qtjvwnpz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzygelly.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hagefqos.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqlrewen.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ehihhoth.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yufzkghu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ehbcnmgz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dfdtdrep.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zxtqvfkw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eixbuznc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2msouplgc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rqiqzxbf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ezadiwko.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2unmwkdqm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pheeyqlk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pamnzhxp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qkniadqi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vctsqenc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ydqsywhg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xtgncpft.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oqwymagx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uxqvbcvm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnrvrbp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2aadhgjfu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eusiwizp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qoekwlal.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rrdddfzt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cbxmarue.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfrzaebi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uccbofly.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gtwfsugl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zvqgfxfp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2aitmlcuh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhwrxvvf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hfsiyvnm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jqgffsmm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2omacqwdw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaiugmsk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmoplenf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2eggwpfwx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2zyzxepkr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dxlfjiml.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bogmexcv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bxogmdse.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mykzujdc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2llgudglr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qmudzyge.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zubbwhey.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zypexfwv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rqytvvrv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tthcmawb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2doobtbfi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2keclmwaa.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2sypbbhoa.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nslvfiyu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jcsgkydl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oafetrzo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pnheciqv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2gkioiwsx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2uyraaczw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rmwywqwh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zckxomsf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qdefmcnc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2kuvgapxq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qgcsxwkb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ssnpgajo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vkamibfq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nmwqrijf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2sfmtzlem.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2cvbndyij.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hxgymiqu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2srkyaifr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2gogplnmo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2izvqggph.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yujgixit.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftbdhsdm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sycdpdws.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2xtlisufr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ylsmcxax.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2pnywaujg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2gbxucplb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2fxdectvi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ujyohtfk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2itpzbdsl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qnagtixn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dhckchcl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2jyxibngg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jmhhyoln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gymfioog.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ftfmovgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgdjqrhi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bvtwplvr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwjjvia.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gkhyppln.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lziwxbkm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2iynunpby.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lrpyqqtt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ftrccljn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lvkvblas.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lclmsito.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jqzabrcp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nsjcbguu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hbzjjcgr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hbwaazma.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jzagoljk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2eupxctwy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2srcrbfwr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zrmbhgdt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pxrlzaiv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2pciqmfpu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqvqkvpz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pgkcpatg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pkxryyqp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2wzihkmbn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kvqggbce.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2isvkdiuk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mrbvfszj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2gzqjxsiz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2xbcmyfgo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2otpunnxc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2pherhfwt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lvcpluqj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2emyjhgjn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ggkflshh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xswyrxte.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nyemjnaw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vmtcoivd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rdmrkwow.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrllspu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2noutgnrj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ltxxrles.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nenmzesx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2bxlykvqu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zspqlfhb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nrvncvhs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ffstbvbi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2giivinmk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hcoupqtt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2phpmonty.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fabpyfop.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2haiyjufv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wbmghocg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2zlarlzuz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2stkdjsky.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kehqwzrk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2dfjimqic.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2mxolfebz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jfefvopm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2yjtxgbrl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2sngcnenr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2fihcqycj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ruezzrhh.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2oolmxqtr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2basqjibc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oxywpfgc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2owqjlnrg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2aotbaeeo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zwmzamjf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ppieunzw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2eygktkmo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2qkcbmxdk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zkiesxsj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hrhnqvwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnsqjjda.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gvvjjqar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxlmvhro.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qylxszcv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2jtazcdlz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qgatsnhx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gruggmkc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2quowhvom.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xklqlrzi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2kulyztre.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2yalyyscp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mnlbtsis.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2lpqxgdpp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2dpftflsn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2asnpocmm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2nityznyr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2hnpfzusa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2epzuinye.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2odcdngjq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2nkpvepln.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2edrpylfn.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2gncmvpij.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2qrxjklmn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rbfkzaez.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uccwhiyi.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ooeglqez.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2snffdqdn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xxrurvbt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2chwmiswl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2icwcyyps.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2baenezgs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ctotccry.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2yyofvbxm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gtvctfkz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2azivvjcs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wsanzyro.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hdoaugug.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xopvfdzq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmyxlnb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2gdqfzhwl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2qvsabjro.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ihyjllof.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rdzvnfhw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2crxzcejo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yxlrrvbu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ktxqemov.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dqwfplrd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gnovrddc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ufojnvzz.html


<!-- 参考信息 -->