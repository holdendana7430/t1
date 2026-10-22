代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ojzbhwku.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ffvtpdtr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2stpqdlmb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2joodvbjq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dvdfwqdi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgvfuwcp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hbqcdslc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gzpjpwgp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jdacjvty.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2elhjoxqp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vdeqgicz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hvacpqdc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hjjvakzr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhhmshdk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2byajcjnb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjvfvbmv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpwhrhxb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2preeluyb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2spfkblux.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdegtfsq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kzurpbpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2njjauqrp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qayddhbh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lsdxxiun.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ltjxztjj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mcudkpxs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gzpgddpr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wpacitqs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ykrpveho.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xierlnyk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2crejbooa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svwnzbmh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbnjhlav.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqvhypru.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulgzbazy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2whifeguy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tpimzwex.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwumlomf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kgjpvjdl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hvijwqlx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fevhwowy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ashwvmhr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ninnoswp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bvarixaz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dyqfytbi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ftfrzlom.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wwhidymk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vwsgqnub.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2btswwkys.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kutdjimn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ucjrzssm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jacflylg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jdmzbyvl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hvgvkkrr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2solgawov.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ccegweqm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2clvienqj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jcxbrwcy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ymyjdvik.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nbgltqok.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2sbrdctwp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umehoeyx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2hdzjtino.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2cjhwpyhc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yflsieet.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2aomswhgd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dajbhnev.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cifxdvbt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2peeeobjx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgkbguox.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wpdkqjhv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2seunvflr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nemeklnx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zxnwnvfc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nxsavnjy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ixuwdzmq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kyafsnak.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jceveglt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lqmrqcaf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dbucqywg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2obdbuawz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zjfcnbmk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dbmfofsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agkhnfyo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bcwoxxxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogukhhfj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2obstjmrd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2futlcpwx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgdlpobr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikarmfub.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zwkpnera.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxdzyhlv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2msliymiy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2typfzrvr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2apuzvihf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nlipauco.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2eakvceik.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpuathhn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ghknckqc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vxfwtswn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zlpphyqg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2bcvrzcly.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvmfypvm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ymenxbhe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yhhrqedo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jkwtpzla.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xdpxvxyf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2suyanbqn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bxpwcamn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jczjhnph.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2braqnuzh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vlkvbtif.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fspkcowr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zxgyivvb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tpgjewpm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zmhlfmqe.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qaaykceu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rreemxog.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hsxxarfa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2hxnbfpbi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfiguvfo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhqnpuzs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rccgchse.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wciewqal.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fgxryobw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wfpyvptn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocbejdfk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2emwpqplo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pogwmryf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2pzheeuhj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2htuzqeru.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2upzzabkc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vqimhokk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vopavttz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jutbehkp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bytmrhbu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wdqrhmib.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qvnovrdv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yuxnminr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fmiwxmzn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xtcsqwsy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2axlgyrip.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zsmvagwg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2litqgsny.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pyrqynji.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mgvrurte.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2omtjzoxg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hxtvtqvs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2elsupkih.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pjitadeh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pbatplum.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mwifzfai.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qiqostqy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2posaqdvr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kdqvbptj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2omiwydik.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hdwcocrh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nankivqi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2uyzmbekr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2osvkdgjj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kkuvxjtv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2unwrdmey.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ngwbglgq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jtljacjq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hirhzyuv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2eejprktu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2drwlrsja.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2pcqhprac.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pdvnxowd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2nyqgdnny.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hnqppqei.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lintpvgn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2umdijqnu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2drontjav.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfkchqh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sulxdida.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wexnpree.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qhbmngux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jefwkckn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2irwookfp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzrztuf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jmngaanp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfzwjyd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2luvxemfj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2oudpetst.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2issfyhgq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2anvxyohi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2irgtvrec.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jazydtsc.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wrkcvtwz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2edxthprb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2cymqhawg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xzoyhgnq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucavcnux.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xbpdnble.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2deenkssi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tyojpwsc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fponshdp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzguqry.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bmtjlmxc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cyijstte.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ugahzbbs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2hvgigubl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2nxbtpmsy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2elnzyznl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ilqfybff.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2hdjqzbfn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2icgnvxow.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2brbjqjci.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hazaldub.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xghrcgwx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2psbkdbee.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rnmkcplp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2koldjsdz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2zptmdeyv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2qptdmobh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2omcxrldq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uxgsqmix.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kqtmnohb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rrdfcqih.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2xahjxvbj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2iippfrhc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2focdqdri.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2foiokyaj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2bkamaoqa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gluqpxxm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2euaeifhr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2sgbuetkf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yzuiitko.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ckuvqwqy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2hxatmszu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gqtkaexk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jbvzmudo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2gnlfmmoj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xhozqfdt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vijlejco.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nuhnyend.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2codpoecr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2xpngjbgv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2hbmutgii.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ncqutmtr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2zgnqplnf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ahsvafzu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2yxcwpbgu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vugvysqd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hxujnnxl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hixbjvir.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yrarxtyu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gyahyjzx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vgzwjzgr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xhvjisud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqugrciu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ybnarzys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pklbpxpw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2yllredyg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fsmlwrfm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ebqvtqtj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2tlgwwfpz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jmmhyljk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hrwjweoh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2seutvyin.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2wosdoyec.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ewpuvttj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jycpxugf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jdtjibki.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zljpnvqa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2lrlfaxhh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2xkuwousp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2usmhfsdh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2wwzvmegt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uzkautsk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2wnsmfnwp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2dbcrqljo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2pxkvdaza.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2zmrwjlig.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wwbbfbas.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gtyqxtuh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qnqerueu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ywloliaz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kmbdwudk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2mabntdya.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2etzpsaii.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ewaxiwqr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2odfzowxo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rfovrldx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhfcgma.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bhhicxhf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qfififvf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2mrvpjnkd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2wrrzrwhl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2kvwyfmsm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2zvvvpixs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2tjcpispg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2itnvxrkv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zvubuife.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2zfxcohuh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wjwscogt.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2yojhhdqt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qwizpnnk.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2fuskmrcl.html


<!-- 参考信息 -->