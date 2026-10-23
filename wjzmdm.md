代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3lfiokoah.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tkjkzoje.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3esbsehll.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dzuwwtyi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bmdfrkbn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3azxibfnu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3puspylkk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3txcmfwzh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuywtzay.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dgcyxecq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kxgjidgx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtnlkqcf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xpfgwdec.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ywrgosqn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3omltnbhg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3yzpntsgt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3egltspqv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lwtvivir.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3apyokzqg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yimphywl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zwwvesyv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tjkasmdw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vxuymmfu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xgybrerw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cicrapio.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pbgtcmod.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zoqtcvfz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rwymxlcw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tretbzkg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocqpxwem.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cvjcsqxl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uhrmdjuo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3domsgvio.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvedcnwv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymetjckl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hiiftxxe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yjazkqac.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3atbhzhlm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ssejiwnr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3luwkuhia.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3aeaommss.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3slqtdgxe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bwamotzm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hrrjzkgj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mtokcfof.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gcwtaawd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zctvihay.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gnanakmi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3krygetik.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3npiaicgu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3oviqduko.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wzqwjlso.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jtwgmcdw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntbbsvcq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fpfbwswl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gyeyftbd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3wnjdhegi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nnsjsngf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykmegwvq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ginmamby.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3iajglgmq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3drzuohsw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gwfhqzza.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3lggggmrk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3eujoqcrc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ngfritqh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mbsrhysa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3esjnsbui.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hjxodowy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qwmcxbeq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpjmlhd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vzcaikar.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3halfxsuh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3upbctwin.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bbyzsyye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdagtsws.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hlcmwitl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqkgmghb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3otllzdmu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rjnwvmvv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3btcdfuuk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hbdyzutf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3poanzmyp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmyqqgyq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ubumgcuy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mqzunwnz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jjrumcaa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bfgpetoq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3stdilytl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gskqkjoz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3avipthjp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3obvmkpqi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulfgeakh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uiduudxq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmjusyag.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3osuxcafv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vlwlzdbx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3freslegn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iixusxwg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3exvxderp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ibpljinw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lrfrkvso.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfxblrb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3myudvjsk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vturmwwd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xhocqcpr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nldxuzep.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aagtuhtl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3owfzvmhu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yuwmwsdf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hjmyjgdd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3soatsxgm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vppgbpwt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jnoyjudh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xpsbdloo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dqrhlstn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xuiqbqid.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bajqjvvb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpzhmqgh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rcgiwvkz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3cuaxspwm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dqwiohwx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxxalork.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ugjjppye.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ceoppujq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gsiyzdhx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cbfxpvkp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dglekycb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bbrlnxjk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3redajqbx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3agagcrlk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qqwyiwzs.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3iubvvrjm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ktvujqfh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xqgzvfes.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gfknmzmc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jjrgbyxv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3nwzcqcba.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bxbnhrik.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3uhlxecoo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wffluwac.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3phzvuoxc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3smxudmvr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rhmladtu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3lzpybazr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pehkffhx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fawogsqh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yhakrjqh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3bpjyffjj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3lnscfmbf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tnmnxsqq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ttmkqfpe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fkliazcu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3znewkixn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xinkcfad.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbtkmic.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jiondocl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgfdrys.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ripxklkl.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3oirbiqkt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3jsbthwsa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3uputbnhi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3aafucjkz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hzpgaopy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3hozwmxax.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ueyuquzn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xeknvhea.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pbaiwdjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guxylawq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3etggndul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwxfzgbm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3bitpkcfk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3emnrcydw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fheqozwd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hqctwjua.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wzbedyvm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dknojsvy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ayllpzbc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kvmailal.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wmdgsfwa.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3lkcjhtpj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3robirfnz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qivwexuq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xnjtzltt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3pghaexpg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3learpxgx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3noywllam.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nagpffxk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vevfsmfx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wbmasnsi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjdyxgi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3detizyck.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hwqqntcn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3fkdkqvcp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3wjyrdujr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ceblkeja.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3gtgvutgk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3nrswxfvn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ctyukkgb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3okylxwge.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wfbbxqno.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qqipecun.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zcsxnmiu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ihjploxl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3pjrjaqyc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cyimlcfg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ydsbhugh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yijburly.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3owwpjkfq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gtkgiwrg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ksuxhuwy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qmchdngm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3srjrnhci.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gzbpqhwk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vnsybpif.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3coggtcvl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ddiesksq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nzehnjmg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ofvksfpb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wbsryalm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3azwfqiga.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nlpqfayj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3xfwbicwf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3mpwlfcdm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3saumudzy.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3xsacikio.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3igpehwvz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nlxjjsmi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3desafnnf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3pdiyhlsk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3swlhunal.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3eljhptvk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3ubjkqjab.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3hzcbjgbn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3idpwimen.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qmzuhtqs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jcsatiiu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3udqusjzw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ywbldmaa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3piqzjmtb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3btvggcmv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ilpjvvln.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3brdqspim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufjhptcb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3fozppvls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atjljiyw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ujgislwp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3tedpinwl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ercfjrrs.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3anbsuzef.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3znpygcgo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3gtknlmij.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3fkvthpxy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3qfglvylf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bxzjuxlu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sfxequtq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3movydqrf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3drrvglbi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3tmhuqedi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3xckbvvmi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3waciupri.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3bkbqifue.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3astscafp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zxzgketi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gsqiwfuq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vybtoqdm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3gifddmju.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nplzcgbn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hcnfsnaj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vqeehlwh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pmddwmog.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fisowfuc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3fakefckx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3xlxkdpkq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvbstyv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dehryimb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3mzuulhws.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkmrmvt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3aznhbjnd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mzznjpfp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3faolgxdt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vcpyrree.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ibdifyml.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzpztxq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3euctnndq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvlujoh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ekxxknbt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qujduukn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3xjfhykqn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qndraehv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnqdato.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3pzvmuqgt.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qtprrzxm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3dvenqild.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3vjgfwsdp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3gacyckdn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tlppnoet.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nohkmlsi.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3xmapywib.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3sdjkunzt.html


<!-- 参考信息 -->