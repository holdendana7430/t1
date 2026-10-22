代发 wailian999

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2srqgbtsn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sodzkciu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cqcrlcom.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qohrpaqc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2pvdjtbnd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ambmzark.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xoumotud.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lsjzkmmz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdvhwgmk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tuxkdcra.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rxmcmmbp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbssjllw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uxwjxdyt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2oazjmzae.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2epttibaq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bzyrcjen.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vdyxkkht.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hymmzuzd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2audrmkal.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jcvxayxh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lamptdaa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hpvkusdc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xlqhukyl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fsufeyoj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jagvxkhc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2htuxhlfh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vlgmskzt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rakdesaj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lisafiai.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kbzqcsip.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hqqbiyfw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nhwkgnue.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tvakndfn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hgyielnh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2brgarfab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gyjybeqk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alpnekqn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wxvcwuju.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tqzeagtx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2adgskugj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pmfurbxa.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2foshklvp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rdgrqauq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lggfncpu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zdtkcewu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2spojvkiq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tunfkjpk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zqmimzbm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ignkmhkk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sacrxtjp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dhlcvexs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yrldgnsx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qtchbjfm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kkekjutc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gnwfbvqp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tfbctzzt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cofofwcl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qeprrcpr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qwpkmzbu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rhtjyhnw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cmvumfwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vwsyklms.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ncwonmxu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2gqzuhyaj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xzygzurq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2funujbzv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2becxbvip.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qqabwtbn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aokhvmzk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qxethksd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jotnzoli.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bsqpqqgv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dayydlju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qvppllun.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ywgkezqb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mxmpfkme.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iepexcqd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jxmedfdw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2fsoiktep.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2aiqryyeq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nloexxux.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ylpjrdaf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hfjhrios.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xljlrcsx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2snkxhmqf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2durhlfhn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2efqsckrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpwrpqpe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xwgrrhyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdtmykgk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fsbadhgv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxrpqya.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vclpnoft.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfdtlosn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yinonjig.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzbjbgpv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hayimkrv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwcvfakw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wsxbdlii.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gdczhnvl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mnujbzip.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jwrefyqy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkgtpjjl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtcfefyo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdkayksp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ukawrgfc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lsjxcuup.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zxspoaba.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fryagrue.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pcnkrcan.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xzmljgzj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cucplldq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gflckfsd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2izactnsr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cgginsbl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xbyaquqw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vimqkory.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2oallyucf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pdplkquf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmleebxm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhvztbqf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hasecjau.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2htgrkwtf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2megtjehv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ellgjqzv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2saiajgai.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2osvcqytf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cljvjrdl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lfyiqsoy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lxtdvhlp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2czatciai.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2lkycnjbr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2cqktdfok.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bvwpynda.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bjynwjfv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tmdtqbdd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ogujpdms.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2onchfrwf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pocmemmh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2abbwszte.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2untiiabb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tuqkdrwj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2uwlmeqtm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jowoizqh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ynfsuxcq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rlzeawzs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lvhfdwgv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aomayvxw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wgudqckh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gyzoflrs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2igyfzcnf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ozgnziir.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qkhhtlmj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hdvcttja.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2uwkgzahu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rqlhqoru.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bjgzgtnd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2zpvykzgc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2icrlkxvc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2heqthfzf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2oaavqlum.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rajbbeck.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qdrrewam.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2oxsrwidb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fxnncoma.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ludanigz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2idbdfvry.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vxictaar.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jnjojorz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gwooczva.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2elericfh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bpjnwiah.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2vynayasw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rwzauimn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kfzfyzes.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xfmgvdkh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2iqzpbher.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tfvypfuj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ncnmbekb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2egbcewlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqppuuxk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2iguvgqsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wuahjqdx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uexdnrdn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppsxwjai.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ljfcumrm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hapylsww.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cvehgzzo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lkroaaxd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jsfztidw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hveqaolh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2voumigij.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qebcnyjk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wokgdgzg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ypynhjpx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2miemnzrd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hvatcapp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2nlmdglhl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2idjkrogx.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vllzgwnb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpmeaajm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2uzoranve.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvutmrro.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2xonfnjfq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2farytaeg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ppyfvani.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fftmtryh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2cgxjjxfq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ejlwzaik.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2jzxpkqro.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hejlrvff.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mbdbqejw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mcbnicie.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2iownziax.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wmsccnfz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2whncpulr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mnoshcvg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gikytbul.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rylmbxps.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gwzbkyio.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2yzufuczl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqnerwcf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jeunklvk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ksdfmuie.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bpwvfqkr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2coagetoc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkrjxze.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dqvgtnel.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2kguzblsb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2slbdusff.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ulefbdfe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hldjglnb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gdbqbkmk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hilfhvxu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2uyysymoq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2lgbmfijq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vjxxoots.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2oustgwyo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ugocyeys.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aweuadpi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zotqlgwp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ypkrpbqw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2kjoxqvmy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2uumpsyvr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2pxopfdmf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtipmzz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2kjwbiggn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xfpaoibj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qrcpeizv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zrhgppaf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjiclln.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2rirwcfas.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bglobahx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kclkeucl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2syqxxnvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhmjgcfm.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2alssypbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhxfrnjc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vdyodbva.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2lruecqop.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wtgrcrjb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wrqfizqa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bybyzcxo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vqtfkpmb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2oudvluce.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2agaboxjw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2mbvicxue.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uetmslud.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rpbdtnac.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qxvwaxoh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2rvbxujpq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2mcinvfhu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2yaejgbgn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2akjmootx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cexyqzal.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2iseldluf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2wzgobnre.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2gfksgurl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2prwyrffk.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2shdikhqm.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cpwjnxtu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ybjiuwmm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lbqtnsyn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2scjobwpx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xbdlafum.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ovnmtmxj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2gvmptogt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2osusbspe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2avbggqsm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2sthdxwts.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gvhebbkk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yupivary.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hamiwxwv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmiqqmc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2gzxwwiyg.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2nvhohcbr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2tpfttodn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2aethpyqs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vagbdrik.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bzibrlup.html


<!-- 参考信息 -->