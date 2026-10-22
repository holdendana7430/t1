代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rjsvcpdd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2oahumwvb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzgeakch.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycfzvuiy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dwcathfh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kyhqrwtn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihheqkcc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2svlkrgpr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2girckkse.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jfhtdubz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vcxdjcra.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tqqwvrnh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrprgbxe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2oigsjtto.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvhaehhg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gzvtkbkh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kqpihxmo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tqnqgkmp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2irhtdbqb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ozxxawfk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xgjgmygm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2oyjvqtpj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ttpxpboj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hiuxqyao.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2atykdlzd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xiatvwca.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dgaekkjb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dykfxlko.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbfzuaed.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zwwjmdwu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mumehmpv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mlalqfps.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fgjhdsnw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rruyvpno.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2byvtojyh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fgtfrmjk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqqqsjqd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xonnchpz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsmnaur.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ihnzlogd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nhbezfxx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2khyittze.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2phcuvixg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jpyofgkn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ydrsvwgv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iufxtirv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fukmkzkf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2esfqmxlo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2feyxuiyg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2aicsbkny.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tddktryt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zvdmicew.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nflmsvnn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2eesncgrh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jfwfcopv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jjxnypmm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lwcjticy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qhtdmyyu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2syjqxyup.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2etdwedyj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mlfefxep.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wasykqnn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vizpxbbv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bswkszkb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2euosnrrq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2aehgmoun.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2cdiplxww.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kombpzof.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2engjzzrq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cgkufclb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zqekgslb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hpflhuql.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fycrsift.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqtjtkxw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mweyqhpa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dsnfrftu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xahnunnk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ykvrosfc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2faesqzib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqskeqjf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ynehntpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxcbzpxv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2simgrbnk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qrjwhrbr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jfuqkjxt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nmyfpecc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qsjydcnx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbynlgjg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2taickxjg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypmmfbrw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lxampnmq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bvgyrzoz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2djmrypuk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fyrcgcum.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kohwbvju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kizpkqgr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdhmigda.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mcmcohfe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yyvybdnv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2leheiweu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vciyhozq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hijfwqbd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pvbswiqu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xdhxcols.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rkgutdaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xfhfhtav.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xwnyqfdh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2elynenxh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lrhobajt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktjyuvmf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rqreskqz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrqxqifk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oluqlece.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wvqneqva.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jactktvl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jilltqni.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ktrmkjab.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbkfgqgz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xeklvuav.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yftilwhg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ljdrmwcn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2byrgwapd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2stnlsngr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rxoyhyim.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2cposqikt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2gnlmwgbq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtyykejb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2wlkckghu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2arcawixq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2chrdkfhv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2enlrpswp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wwzghquw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mszfuszb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2btjqinqw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2cqbatamf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fshllkvu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vxgreeyk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qhjfunhh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rahwecgv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pmflhzli.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lismvrrg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gsbnlmqa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mueermbj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2foonttno.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yprkfpjn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vbpfeyzk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2souhryny.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2svkhmziu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2pmdgsfby.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwectgp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ffrhvrum.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2djxtkmew.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2stfzkjvm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2cnfvehqb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2osyonzio.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2seuzpyyd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fadgqvet.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vfqzaagl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qfgyhvbi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zsxjwlip.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2atlpewua.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ixkxzacv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hygmxvqa.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2owwwhfwc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jmjmlgjk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2edkfnqei.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mckicedh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wnjkuouq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2qkfztykx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2pegerkef.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vzjphjqn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pkqynwqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loyoujnk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wuufesdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzmdlynp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ufmlkqko.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukdpkfaq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2joqtjpcu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scziueoq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tnxkluoh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cndfxeqe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rwbmmftt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ieuifprp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qewsbpwc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2uruhstsk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dksrqnul.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2euqqkqhi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ihoqflnb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2itygiayd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2iqxlxeva.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tmobpcvq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ukmktiir.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qmxzivvt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wtsnzljg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2qszjmmys.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kdajrfaz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ycmnwibe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nkrhkarb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2efpjxxjo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2sczolzjl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qzndtddz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2atphnafa.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2aelfhvck.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tyonmrgx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2impzrvem.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gszikdbj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gljorecv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2neusiway.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2smpulidb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2alebxkwd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zzsurkyt.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xuvuvipa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kwkoyvwe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kbzqhqtz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2umrzjuxq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gqgqcxwy.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kkbkfrlh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jtwyflkn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kodlfmvj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kycqpzrz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2irrazlfm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wacgyxca.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jgveerlx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2suacfksp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mfjsctic.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rkxvoplb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2crdlfoha.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2nfomdams.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jbojaxeu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xedqyund.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2scaflpes.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xqtjbsho.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2vnbotlsl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2etdlrxkq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2acqzngbs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2vbzmacps.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2rhksnwfr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2besnhdcx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dsmohpub.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xlhfoxlt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2clymmyws.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tgvkpcag.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xbbdmvfm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hivpnblr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2pbirrzav.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2brqqpgjb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mxlvroor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfkdfxti.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2npfipkxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkydjnpc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2bljdxqhr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ziexxxuc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bbwnbdvy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2pfpbgroq.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qjdiwkln.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2cadjjoeo.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2obsgtpxo.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2linjkztp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sygjovkf.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vrhxkmub.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2joydshma.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pdjudcxh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2iezlxett.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zfirgkpl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2lzcvgnfh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2kjkaakwd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2sosmvajl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2znlcvhur.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2nwlshqlg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wrdzfnrp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ksszwaay.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fxgtmnqu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2draexjvs.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gcjchlci.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nqpeqblo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dwayoken.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2gadznwwj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2fjwfejsc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wgilmarl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wnysncad.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gdatgime.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2togghnjv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bhnqapmy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ztuensvo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2cneobxpx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2oyujyvxn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2gslbnmnk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2jaudnsoc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2cudrkbpy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2eausmjfw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hpsmvppr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wqjrmwqa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nlapnwrq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2bhstybgi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2eouvybkc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ecjnjugc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xismayau.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bjotywol.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2gkmcmbrs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2lzmpvsfb.html


<!-- 参考信息 -->