代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxgwiwsm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2krgkpdch.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uotvawpa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqzxgmdz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pslblwel.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zqercuac.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tkxenxnu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vaxruecx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pgqkbmzz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ceozuapp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2phpbpqov.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zovaeepq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tdlblyio.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2edwthbpi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zrpdqpcu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2znvjxxly.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2btdwlmnl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbusxide.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oobnlgeb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ygswmtrl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mrtzgden.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vtyxrula.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2aqnpvfsk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kyhgpodj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqdnefha.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mctjvnix.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pywomytv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pfimyphl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tgmrgiio.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmiagzam.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2okaleshu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2drxboewk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oewbfnsd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lcqsrybq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hpqwwanz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qogyyoiy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hamrdbuw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fgrrddmc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2oycftwpw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bavgyqon.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fptivkeh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2oodpzziw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fctgtbum.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wvzayvin.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qojgdiie.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2guhjvnqe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hvjqsyjc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kodscler.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2sdgvqsul.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rdlivilp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vscrkxko.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zgcxodug.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2waqgvjnh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jqairqwd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jbrmnzhj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nhcvpkzp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2vjcjulkj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjokcue.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2elzurdon.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2fweraumb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tkavweop.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2obrocofq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tyuezxpi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2clbrqqap.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2eoafgbvi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2gaoxcgfv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2maidpwph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhkfbjxj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2owpwaxbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llhfnbja.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qtafffls.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yuvcsitb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zmvpqbpl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tmcrmuxd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bhytorkl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rksaawgb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hcctfnmp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xqvtpfvz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ofploscx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ftrxjauo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2pcnyldtu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcqiscof.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jztafidd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvdwahwd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2agvhbgdk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2sjtcsgit.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zsoepqjx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ihpuvizd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2unwssmfx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2oyvkiqmw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vgmaykcp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ahvwwzpe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tnrccmam.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2inokrukc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wyqorpjh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ugtyyeoa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pifklmff.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vesgfoot.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mfhpnxso.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2omqmmjez.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xgztnned.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mykmwauv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hjtzrhzj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ohapmpxl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2efhtktfc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fatjervb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cshvuemp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2mpzrvfup.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pswbygfj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaalqovk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjoynplv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ritwbjyc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vekyulti.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2slguwlfv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dhunvpmq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2gaufvkig.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kmvsnixd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cbidnfci.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jhjifatb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2toxfvisy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xggypvsd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fcwuvvxj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2quzvybuu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lsjfjpje.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lhlwnjhe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2golcxang.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wnfbfqry.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2snasbicv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wytxveam.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ptxtqmgg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2rrmalsft.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ayvscqll.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hagjyqri.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lvzdylbt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lckzgoho.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dotcyvyj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2fuqcdpqn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2gztdlqfo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2brpnijlf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hiizutuz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qoatstpq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vkyoeovg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2joaasgti.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ouqqqkvd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2cwgoiqax.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ikrjxjsh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2elphhhhm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2jscrfkkx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2yaecowqj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wddsujzl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2tzttlplw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sabuhgnk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kubzvkux.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2eguijrpp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gfakitbl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2isynyahb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2siadfctu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ccebiqal.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pjtfzhru.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gleuytug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyrninia.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kukidcyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiwlkzqp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ctxaysud.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gpvcgoqo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iajgjyet.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jsljgarl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2shpwiwli.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2oqzkdkwu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2pfosgwfg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wrvhqmcw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mrtradse.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wdtqqwmw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mnqozdpd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2khhmwyqd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2woomxrkb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2iojyowxr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2hvyyuqdy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pxnhjffq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yidafzxq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xxxkvkwz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kuamkeem.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mchzxrmx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bmnfdatw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2obucqewj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ijnxahcx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fzdlpjrh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xfvtemmc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gczqfnrq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2dzdxnrvj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnxoihyn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ordntkpf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjsfnatl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pssslqgb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uxwuvcpz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vojrsurr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wtwnosid.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tgkvvyhd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2benztaso.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tbmshwsa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2fzmvkvoe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jucuyafk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qjblnoie.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ufjquzeg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qffbsbsi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dvgdyxps.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2brxeuvui.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ajrxgdid.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2hwoewiuy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gwzlhtzd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2nhlclokr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rrynzrnt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jpkskcff.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pnlhelbi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2oebrjibr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hfzehcaw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yqvmdzcw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2dmxngzas.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zptohebz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hybklegz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2gajrlenm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ktcosdsz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2duluhyyg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhwteuh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jsfoociv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2liwiubhy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pcbhzgba.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2chrlujtn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2rzfeqzmr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fdikcsoc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mbdctqft.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nzrrezyz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2uxvihodt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2bisyxjlo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tmgdlbzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmcrsejs.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ivzieljc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyvzewha.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dpuklvos.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2nmbqwnev.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2oaxxzcwh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2apneqgwt.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nqbxmsji.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2yzjgizgk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ukqudwgy.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2sciqqqtm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2xaococdi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qkxqnfbr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2exoxafaz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cuzuhaqx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2mngirfqs.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wzylzpcs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2dfkzwrmy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2mqsyfcsu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kkuicqcx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2cywxkzvc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ncyccfsq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2pnyogxoz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2vddigmhk.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ieknngwn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2azyifbih.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2spcxhyqe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2arzwtmju.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zapfqfhg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pmbfcnvk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2qksvelqq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wtxypmcl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2vhleixal.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gnocsvhq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2mfgpdxcs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ctgmqhfl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nblidjgg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2syzkkezq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2uuschrcl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ywkpjqxb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2leilbppo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2jsunglmz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkfxecn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fiaeckhz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lrcsbpuk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wfrcepyz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2hpqggcwr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qohejvkw.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2mqwjmnnf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2plgrzqdo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zjksnbcz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xzuksvlu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2sdipxnsp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wcksjiej.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2kesiuxok.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2sjspbeby.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qhqworzg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2cjuzaxzz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2smfxrzmc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2grvjfkxk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mcleeeod.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bwsijvnw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tedxsvtl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2fggocott.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kfjyyeld.html


<!-- 参考信息 -->