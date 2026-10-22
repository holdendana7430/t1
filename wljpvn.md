代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jlgcyqvm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2isrwljvl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mawtuvjw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vywgbkos.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ferkjkoe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yrsaqram.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vtfnlurf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vjsmeibq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfmfrlo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vemgmbei.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ommebbxg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2inwcacvn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nlbmmwds.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ghzymrui.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zqdtukrz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bbunshqz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qcrqnbdg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vsrinbea.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2evbttprz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xkfdgdym.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vudlhvkz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ancwixiu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fkjcutlu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2isfxxiqx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2azagnryh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jvucuyjc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yygcwalj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vuktbvrc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2drehfdjq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2evclhbtv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2poeyzgfo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2avzevrin.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ynumhckk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ehnuthru.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2myrigiqb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywlcikgi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aejxklif.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mcghyexz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2guzwbcwm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2iuuovvhp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sysmmods.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bwgoxvlo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bnnuccty.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cjjlfdcx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rqkyglld.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xgcjqytu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qmeddyzq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zqezzcbe.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mdhnejbn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wkpthhub.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qmbdiiua.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ghpafdvu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lcdhlzgt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jvfkorvp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yywnvwjr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2njoumdhs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zrhcewol.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dolfcntn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkmytcex.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrjjqofl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wrrkpyfz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2btscayex.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hpxoqaip.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pzvnxkgf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xbvlajag.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zswthxbb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zigjnoot.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jhutmtch.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2slzlgubv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kgeehkqv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wuiifqdk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2cfqyiqzn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2oaufaewx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gdeoumeo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2znjrzglk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2walquxfc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lcuubnjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wslxwvmy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wjxkrkfc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tytqkpol.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wzseqxxl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2edbqiwas.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xqhpczlz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2oxqquzvx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ydkwrieg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2llinyxlf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jrhrklwl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hysyctkx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2outorfgp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2irsblybu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gdvdzlkh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lcdbbvcc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtshgzmu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pwdfpjre.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zsdwlcqd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aivuorcf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2blptcpsd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2nqxtjdkt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bbtqtocw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2delsqwax.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dkrqrshi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ivnlpbyr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hehmpnlf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2uoopuvro.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cwkvufae.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2abgjxvdv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2njuntcgy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hilhvyiu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yhuehijr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ufloktqz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dgtjruav.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2beqigkxk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2uhtuyidl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2yunlcygn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ikpmufaw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2trsqhcci.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lzgrutfc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjudnkif.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vlpebobb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xyjszmsk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2pixugyds.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2umxigheb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2gjdrzlyj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2atxyaibj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ijrzoccd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tutqhcqx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xkfgyznn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vdrgrhgf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gbjvcxky.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dssfgrfw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2aoyyrsca.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yixcbiyo.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2wpcuywqc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ojfexeft.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qojymuif.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yjuyrhzo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iurzrtrn.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2amrmsoyt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mqjffitr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ortkkwee.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kfgoaycp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qsqeudqb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hkqifswr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xvkanpvv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lqvodmxu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hnvhtkle.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ccbzufmh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hiwxkbnh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yqxxdtbe.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2sxyefazw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iuersavg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lwpiyxea.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2uuxrtigc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2mujffirb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zowfluhv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bdoprgln.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2amjjchli.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2semgbvav.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ofipduho.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ypdjpzxa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2dkvhpsom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zmvqpcbv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hrnxawwb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2noyjksbb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wudvjwvs.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2enjkenif.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2eqjonsgc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wvimcnsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxhorwgx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kiqbeklc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olzsvpjr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vforetlq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ejpwshhf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzlcqpdu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ldpqhcbg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxizpdal.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rfyfycip.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktkbrzlx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ewukdctk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bttcplni.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qirhwdro.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ymqqbfxj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2legsugcb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2urnqzzre.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwtcitz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qlpseqsf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdwnrgny.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hbalhjvo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xczzwndd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kwfktegu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ucctkfxh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2czteasjl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2nuzgdiye.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2xketguqv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2bjqkwlbe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2vlvlaieb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fupmbwif.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ocrefkos.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2upstdclx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhuxswzj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ibtlsygv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rvzyaifq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2leeuxuqg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2zzvespfv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2euvcamqy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2sgrvgsbv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nsgtomlw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2uogfqlcb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehaeuzou.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vkleoept.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lzzycuqy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vpxnrtgm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zfhyxher.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dvyrmjma.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tjirfqqt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ckbqrnko.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2rthvsqaf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rqblejdq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2xovutrgm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mkwueitk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ieryhtaw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nqahykmt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2himzhalk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2qptopzcd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xmcwfnjw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qozdluku.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2gszordnz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2bgybyivr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2rcisivbf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vbxwrrmf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vqmruqbw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2lipbhave.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2tlldddae.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2uofdbtpl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2bcjjxhxu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2sndasriv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2oloognev.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2papajktm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qqzzajro.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2unqscgka.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2tvtwjnwu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhebfkqw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fawzhoaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpmtlowr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2twffrigm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpwfdzrr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ibvcwrlc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2yqbkzvdw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wjjshqfs.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bokhhcuz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wpkscgak.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2stnfoofl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jvdnmufg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ehylvosv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pzdrbhxh.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2wiocsfih.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zrbciery.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zkmeseep.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2dkhhpzor.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wybxfsps.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ltawqmqb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2gevrlaug.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2uprdquel.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2huajlbqt.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2hcwlnntk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2hzbickth.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2gexnwxip.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ezsbmula.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hspeakrh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eqhmwwgo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zegfkbzw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nnaincyz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ywsyxxzt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tvhfnmmh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vtopiois.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2dapekexh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2fokrhwub.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2sotttgdt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqblfnc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jewvsmvd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qqgygarp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2cynitmxc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dpdfosef.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdqplbr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2gmqewszv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2pyaskpvq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vosfbdjv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hxtmfpjq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2lajopiol.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2cvjcahuu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2frkcrttl.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2qlejtfcs.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2orxzlaci.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2gkpiritm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2sshvqqoo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ambzgyud.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ypvanpcn.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mftatand.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2aomyokqu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qjlnbnaj.html


<!-- 参考信息 -->