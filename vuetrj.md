代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3loolarvw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kcathwgj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3relnwakv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hglylgty.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kdvpmmix.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lgqwincq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jciwwbof.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3umomvzoi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ibvoxxik.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmxtovnk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfbidlkd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhkupurp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qrksjree.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3srmttpmu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zevavuhx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qhbjomku.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3krjvcqnv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3muplpvfn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3seiviluw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kaioxsjs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zkemriko.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ofqvdnxg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tnnsfgop.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rvprzimp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xptfpflo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ypeoilly.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3luwbjgrk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fgoooxvr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yfxwpxbv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hwejxkjl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bjpioqmq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ctxhodyj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3whfujitk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3snfwmcos.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wevrsuds.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nzotnpho.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rvqgpigz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygbeiztn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mlmytjeg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hnaqoyps.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vfplfasl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3iraznitn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xlfuxzai.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oswcqkuz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3quqfkrqf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljmgevms.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwruulsw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mysqxcph.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vppblhux.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3etiouyhr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nysmykut.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ebgqwimu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ywoqoeil.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zmuqmpsx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3besprhdt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dvakifnl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ewzbqumn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jjunalmb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3msquaraa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vuzbtypg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tlbhkqgd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wyonjuqy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3sufskzze.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bagrbfto.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nmbtiakk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qvwtzoky.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dmzmtaye.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bkzkacxo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ivipaugk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kbfcuxsf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hdblghsy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bravunfr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zhuimvli.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sblhjeaa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3smrltgxx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3weuvrmyf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qakuwigm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3taasqeny.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uspqvjvu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gjglurtn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mxxbkhto.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lvbhmjld.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yldirmba.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3glyskbzg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lzgfwghm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xehghhbd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nluqrgkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkywfctt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pbayofro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynxzaler.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3anmyaidc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tuqttirv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uklzmqxt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukylufss.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3avtjohqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxxtzvwn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lrxmbnpa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pchkuhnq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fkackwah.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lalpjsvh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vssrooht.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjcbtnff.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ahlcaesk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzfporgi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wuhvgohn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vpgbxbsn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fzdqccuo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hhvrdxos.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3umtmngsb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3agbstjhl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nmbcwqwm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uboapqvr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qpuefwky.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ocjfuhha.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dvzivfqm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mkvicsmp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oiiyaexl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbyffkpe.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nbkyhkqw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3shqqhgxr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xljykoyu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rvgmbzsw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zkkylegs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3oapikzir.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3hsatjbvp.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3wxbtwhqi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3veiikdfb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3cbuxpbaf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3njoemwlt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiotfyyy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gegmnggv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qoivaszq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jsacbwsd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kimuqdnu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psbmbnow.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3voqjhpjs.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jlgrgmxy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fxumgaaw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3oyzhcdtz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3semqpfxg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ygoimqeh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rzbakxja.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jxiksnmg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ussdefbj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xhnuxhwf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bofdzklj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdgcpeqa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yyeuxnik.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nfpsteus.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ozedoxbv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sapfwuma.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qulovrns.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cmplmdpe.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3axedutqh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3phqghmfs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3venrmckj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3oudcczic.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjkzzcw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3jdqnjsvx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mdvlripf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ubohvarr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3bkwzgarq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3rpjgcbhy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zkhtrzay.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3mztajfen.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3tdivscyx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zpvbobgl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jyqdjinr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qicpnhxz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ucekiucv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ljrhxhio.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3uaysttcd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lnymbnzd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qxdscgaj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3covmywjw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cmvmcuen.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3kkaaaxeh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3zotfxcrt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3bwhpwfzv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znliefho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkplmbii.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cfouyjon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsmyrvgx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3iwywcdof.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhlxjnq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jxymkqxo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ceqqmyyp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nuztsgtj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dpjjphza.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obwocudt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jvopjohd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3boszmzwb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uygenkgy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3epgvmwhe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ikepxahm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zdevkbcf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3frwnpnqc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zsunqbzu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jfyzvunq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zqmwqbcg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3namkovhz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3nrwkhkxo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrjbryax.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3kwkvtmqq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jlsgahrk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fgocuxam.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ahrrsmde.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rdiwaixm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3tybplgnh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3kebdwjsb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pxwupuke.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3julcsegh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3srbmbojm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ubvidnkt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zsxocwre.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nasznmms.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3sezshxaz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3srsxvhbn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zecwaorp.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cwmpgxuo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3gozwacvn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3twpcdvng.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vabwvbyq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qkzbbgki.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3pmknqhxq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3soikhuia.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hyiopvpj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3mhosnrjv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3cmephylq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kthbbcrk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3unedgbtb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bmfqirfg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jhdgzqoz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3azdsueif.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3kapyyxrg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ipkzsyyo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3flwqgmfo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3cugomusa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3wpdfiktj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xmispwlt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3rvfshukv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3tyhalddp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3akprxkwx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3lglvlvah.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3piyspoly.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3wqkenrqu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3qthixlum.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3sboapwcy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ssrcyogh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3yrahzdoe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jaszcbbx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kegrtiaq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3stwwpaht.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3fvszvmkj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3dacybojo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejqllkbj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3hwfzvygg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdbshdlz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3evycvbzg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3fshxaufc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rzzvdsbk.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ezuwdcgd.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3iqqlestj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3rgqshsbg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uyvpjqef.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3cppbwinp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3kujemnzr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3awuozkhg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3idtxgixr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3evhqpogo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xfbjwwhh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3gnvoqgmy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3blwoidzb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3rywgbdxz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gfhhgbbc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fqlszjhe.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3qurygqeg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3hbbvmhyw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3cmejcafx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gejxywja.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rhysgnnc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kdmijqlr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3owrekvfp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rboxjxes.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3eqskbjpn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kzjxxaea.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3zffhgyqa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3uytgvsgv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vwzkmwse.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3edivhbhm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3kcsyxtlz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3xwvvzcwo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fgbypkkg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pwpuwqij.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ecjfugtd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3knaktkiw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3axaiudzx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cdffsrrq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ubzpqaix.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hsloorus.html


<!-- 参考信息 -->