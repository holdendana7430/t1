代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sohvechp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufgybkpx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwzjgadd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3eflinsqy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3gsjoxadw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cgjtiszl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3msbpfhwj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wuyqcbat.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3furafxbx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zltwuwyn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vkhkgwnu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rwfhdmpz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xutfmjdn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mxtcutid.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ankhsvmw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlxfkhaf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pwfjxvce.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vuqgvpet.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zffkjkxx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3oqsawfhe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bdlumtpz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wbkovhmc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nnqrsxak.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3awwyhkdu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3sukxjtfs.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mlgwyvlu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xviwazar.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lgeonujo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qodbhtne.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvfxefjc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbmiugcf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3avanwjik.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3znjlbpgb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nelnuzaa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ragfefjp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3flitpdea.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3avrpylde.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxgeuwce.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxqhktgy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuwpzlwl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3brdfjruv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fhrlpbse.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3smcsvibq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jbdpjprl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xggcmqbv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gdiuxvxb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lewdjccr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3thsakvgp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3erwpjwjn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qqbpstlo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wjtbyrdb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3htknddnx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ikrpzbhz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xsxeqfpb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3eunstjzv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ihxozpvk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pvbsinpz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dclffgrq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cjywxykw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xtzzqcik.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kdijnftf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tsjhpdjn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rrnascsy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jglqjqss.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lulujwzn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3exacnyth.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vrmyxnqf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3cvahrshd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3sjungzxj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jqgpglyq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3osomiwqb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jbcdezey.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wvhanigg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3clhgzrov.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gfkqpezc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ogthujfu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ieawabuk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ahekbvcr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zfnuroxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arvdelcx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lxfpzxck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfxsqezs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jyazzvvl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3akyihxqt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qrkycnxc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qybbuyrg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cvzmcgvm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dlykkvyv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uahbbyya.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qryvpqob.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyddkoyp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ckmmycqh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cmyemwzf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsxruymq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3syzcpwtt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ebymdwiy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dyybrrlk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wbpxldok.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lyluzxpd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ibnchtog.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vhqzvbqq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3aybwpfvp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3prgbgkyt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zyxopzdq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pjilrkzo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bjxwsslr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vbqimuwe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dohkrwke.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wltlilcz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jmqogxlj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uointhtz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hscdlnjd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uucopbjs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekabkfgm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wnvxadif.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bgpblzjg.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ropiykzg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gekukgvk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzapubzw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3unawnong.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tktruglb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3unlmctpy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltajcjtd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dowtszvt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3psufpskg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3crkyedsu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcfhhiqk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3gqzihfbp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3buccsxxb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rghvbaak.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rhkvsadk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3admsblgt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3orcfxtil.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3afiiedgi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ddzjsspr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nuxlqzfv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3imxyjsby.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ebvfwzuw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fyanfhun.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jgyitqqk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ogvrzilb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nrqmotjw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qmiggcpl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ivpmkhhy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3okoxdnnx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qvdrvvvl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wkjmggxh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3vaxqkdug.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tknifshl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ndzeunlr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xjlpqscp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3iwztldxg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3cghpvrht.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dfletpyi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vqbnibad.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kgeijoxv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jxpjcbbw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xhazbblv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3akbvivkw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgianfop.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ngzxutea.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ftkhrbjs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rwggldql.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3htkxhslm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3odaohjzu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3sibarpbu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jyxuyjqb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rooimqys.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vscaztrt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3llwqaesa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3suztdkrq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okrvrbef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntsdsfph.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tgudhetk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfshkrvv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xyqyykmc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wncemvzy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mpzzadql.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tcesogju.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snaqohoo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3corlfhwu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzebemp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pvfufyzo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lvrltlfc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wvbrules.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dueqaanu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wzyjptgz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zzlojzcc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3epejgfzu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3tvzmmuez.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hosqarrr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qfdmkgiz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bnfgsfvw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wftdbwnm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wjrijshk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3erpaevuy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qhshsqnz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3sabcdfrp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rqwmkdre.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vcyfgolk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hriueayg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kvlskcmp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3xexlzhdi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3jvaykwek.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jfnztlav.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ogspvdyn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3uslehojg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3onrjmqcp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nvrqzflr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3efcjamtu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fwhapiuf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oaoreckn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3btucbgav.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hoyjxmdc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pqvfurhh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aazyuqoc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3frlolwvp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3crspzhys.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rdxlgqgj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cokgyfha.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qyzenggw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ievdrmrn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3eswbbtcb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3cvmsmori.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3wxkscnsz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3udufgmhf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qpxgtokd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3mdayzyvt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mvsmgfsx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3tapjaill.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmlynxu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3osykyrah.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3llgafmht.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ulxxtrvp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ocewxnrp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3dhudtoiz.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bcykybpc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjshaiv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uqesgxrn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qfbotcjm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nyfesbqv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3govyrcce.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3stdtysyl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zliptwvq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3penyhvav.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vbyfzlft.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zrvftevf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zspycnuy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3yhurhiut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzlgrrso.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3hkqjcuoj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tvedgueh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ivjojifp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rjzjubke.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zgktiveh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3tpjykytg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3uapkxinc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3txyfddlk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3sfrknnob.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ugrrzbci.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kkowrkds.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kkpxbgyn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3fpubzkwi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cahxpamn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3fjistcdw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3nqcibfpt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3otldwuza.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3kidclvgp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3lfwpfvfx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3lbxfyfac.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3euzgwrxr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yjtwlanm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kthnwfkw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lgdxvqqz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bjkimsme.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pltrgwec.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3nnprtjir.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kprqjbgp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3abzhgnmy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3iyilevqr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3uqbknnht.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3povxriys.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bvbvnisp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3vkioddcg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rqmzlvhg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3pesgskaw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3czvhpdrj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3gcxviewt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jpreifff.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3dferrmkn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmsdjwl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3skkzfvlu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ndabgynm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zhjlrkoj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rwghvcwt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3sqweazjm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3kqzvtqfw.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3lpjgzjie.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3mezbztxs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3sqvzecqj.html


<!-- 参考信息 -->