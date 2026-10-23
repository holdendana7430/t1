代发 wailian999

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wxdzvpxo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bwccwwun.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dawtfjze.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lwaplyud.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ioitkxwh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vcnwwcjd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fgcoqbkm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvdqwepo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zavuyjrb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mwtpezxh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqnkiqdz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wtvjtaix.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3uoevtknq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktpqovfd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avnaubwj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3coxldnvp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swwisqwx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zaaqcxee.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ywalbeat.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vggnymyg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ndvkqwjd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lsifyotd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mzdxsilz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3iyeodaze.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3bfvupuws.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vdyxcqxw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3maektfrx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eprnpikr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gazzkwpv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mcuyxykx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3oomtlteq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ekgjlkih.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bkboihxu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mifamtmi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ukiqqtmj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3foncttic.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nnabujsa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zubbuzot.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3axhxcbdm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qjpuoocg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wfwrbtxg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jablxmcn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uclmhlgz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tprylqum.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3cknbnifu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqwbmew.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3phmwxvqt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzpmjny.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fwnxulch.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uhayrgzi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pjzcpjmj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3arsmbqtx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gdqyzmdb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bkeiuvry.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3znspbllr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3amqvsqys.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3hyswdkyl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3paqftkwq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tpayiznp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtzhfpsr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nswatzus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aknabuay.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3apiaauza.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3efjzeocf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rkpnkyzf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mbpzeljn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cvdajpye.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mipxrwet.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3aqpvidyo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cemvguvv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsagbpmu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zihmldyx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ufkwdlkj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yvjidptk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rymoantm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvkwyobw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfdwtuou.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sxffmgva.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uotgybgs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3auwmnglr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rinqdzec.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qgrdgbjo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jfswrgmx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aubbzrof.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wrlwghef.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kljvpigp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gsfnihep.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kkysrpcu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hjiqgxdw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cjckqtqs.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mldsnerz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuavtwrv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3itxlskrw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3aufblcjk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mdfzcblr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lphzmxkr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3flgurzmq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lvenraal.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3guswulyz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fzdctxgx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3zxvtbjzu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jrxvjihr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgrgcyfn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjqexgii.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vvsgvqgt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dkxomllv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mmdrcvqg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3srdsroak.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xrzyabnx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fqzjonvd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3snlylrdw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mdbmnyup.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wokeuevs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3txgikqpf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xdmjinry.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3nogkbgkh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3owxrjvjw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3jucypjkb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xthggdet.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jwpuocrz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nvzdkecl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3bhwwhwij.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3nxcolouo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ftpeqmcm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lhvnvxvd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gbvnimza.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3alagrluo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xobgkxtn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wekyhetg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wdcopoid.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ybyoqijk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3vojffoyd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3hwtrrsvn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xrxmddpn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ygypxety.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3getbsobk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3brywqbkc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3diwxbibc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3njsdygcl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tghkdzkv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xdisfiha.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrcqcab.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3lkwfbfwx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qvnzevtz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3tymkrqvp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nkprvdsp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lamicufe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dobvzfdl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lzmfvazb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tyjcluvc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3eeqbjyqp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tauxfofy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqurdofv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ojolymwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfwszcnd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lgfqfaqv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bjkwjnzt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehznrzpp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mclhjvel.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uqdmkcob.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rceryazg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3axlklipx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xjnibjuo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xybkncjt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rakyqyyn.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nviqpxnp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3uycngkim.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3srqwuefk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jjpgicfv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gdzlsbnm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjdzofil.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rnrtqtle.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kwugkthw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jkmzdzzw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yynhoplr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vknkvkef.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3vdmvlosd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mpzcpbuh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cxvuydgf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zzuzpwqd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lbrnyahp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hirrolll.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3piihbexg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fthmqbbl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fsmtobfz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jlhurctp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tlsjirkf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ydqynrcv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mrtuchil.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hndctdqt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yryawoev.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3eqouyqws.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3qbsuxvpq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qyvogmdt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrixjkms.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iaovjozs.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kiljatfh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3abdjlxxy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xbjjtbyh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3gsmuduzy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ihbywyhz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ejdkvqkq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ppjxrmfw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gdaqoncx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3eafszihg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dnmdyapf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3udonncuu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3cvlffhwm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3entwwdek.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xcqpmtar.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3scfqdewi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ywvvagaf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3cytoyonb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3pnjqdukv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3smyzutwg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3uallvqhv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nnnmuqgh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3pzvpmrws.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xxstwbfq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xkddulye.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ldyutgnf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3kqvrcazi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lficuwus.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3oxohcveh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3bzlbemqm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3nqbimfql.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3bysohhmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgqbemsu.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3euptuxqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtqdhaxo.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xpwctcmk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3qobaamte.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3cvwmrfmv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bkfqwnsl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3usuqvrvn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3qbjfpnrh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lejrippz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3atqfspeb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3kyhmwljq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bpboxzyg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vposwbgu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3clwhmbsw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3wlndyyge.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ccpqdzsa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3mmxildqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3izwkhusb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3utrupece.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hlbydjot.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mqaiolqq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3degyqtyu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3yqqopqly.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3molmrgve.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ppsrxcit.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vguunlig.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ievhrvuv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pdohqfah.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3whtlbebh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jpluosaz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uelthpcp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3mjkiomqb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ekrpbhdx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ufebejzs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rpkqarzz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ogifndma.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdcdkdt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3gieloiht.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3bhtmkvkq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3cwvozfcb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3kymcdrmm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hksjqisv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzoodot.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kuaiyvjr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pcpnleft.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qxromlmm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kkjdnory.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3eohynsud.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3uriguima.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3nyikscra.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3vcgodmes.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3bmsnqeos.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3eooxaioj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3udxjrlbl.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3kplabmhg.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3swteumkb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3itedjqks.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3idfepfqy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3mazlenrh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hblkihge.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xmdagjzr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qaoagddg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3nwsiagsr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zsdfidgz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hhpvjejt.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ynodffpg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3bcaciyoi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3gokckfah.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3xigtzpbl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3janurgiq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ukxiicqt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3iggwdqst.html


<!-- 参考信息 -->