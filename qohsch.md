代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aamytttk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqxzwtm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqfbzipv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdcgagtn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xedqhrlk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcmqkxqw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mwzmcrvb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vrroglpi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3haxzyynb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mnvrczqa.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pxfvtzhl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3djuyiuav.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xjhgqdpy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3onwnosqo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3cutcpgsi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rmmucxxw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3exxnnhiy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3agabebrh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3woygdhxg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xksiatha.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3aefmvgmc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehovklnn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3apefogtc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3igtkdngz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3snqweshs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ossxdwzq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3poffnrkl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hoziewak.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dawyxziq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3znvjqenp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uemzadwu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ilwljnud.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fgdldvgk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dihaamwm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3butjdqdd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3onfyfnql.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ghebjbpa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bnubfadr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ktilrqtg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ugsvhphe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ykaizndo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dfouejlg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uinvjgxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vszmtcij.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3budyzqwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3genszuhv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ypkvlrml.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bofkgdvl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lfrxipbw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtdbloxx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vhhahuks.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hsqxylcj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ojcgydyk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rokwrfmf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3posaznrs.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bemfeogt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jlmxaaip.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ooqjkvdc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bvmfdptq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3npfbumnl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khzvomfv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3qjmsdtqb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gjwgtovt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmjhawy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zpufoymh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rlbfsrgl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gsyxyzij.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhosrsba.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3txvoimvr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xtfldbus.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3lcxhgrll.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3efbenbza.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ddyjmiot.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zqxapkek.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lqbdrnoj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ffljtowe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmcpjvkq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrelrles.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nggpzrbe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3cqgxctdu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ohpvnqab.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3kfgbzsra.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qjkblpne.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fbrubrhg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hagtvdet.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ntvfondz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hvdzngjn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nskiqjca.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fdobrpni.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qgwsojcf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dktkzrgi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rupjbuva.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3cdvwbpda.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fkwnpojf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xvzduhni.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wdevkpxf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3kusyxvxs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3lwjobmaz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zraclqfd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xbowuuvp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3nmsnwxlz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3arldqsel.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3alemoxay.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vedatzvo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rdbzfukx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3sbbgyjdg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fhqqnglv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ibeoxycb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yerafwbv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3dsojimhs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ysngurzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3yczaomne.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ywhowayg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qmverqdd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kidpplmz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3xhakmijy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ovvpyavv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gflybfbt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3rqdtfxif.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3pnhlsfvh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ogmdnccm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jdxvqpwu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3cazjxtts.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3obsjlfdo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3uindsdps.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dkxaoagg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3riqwdleh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vmqwpyqa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3tkkozldx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qmpooivx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nkyfrsju.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ulzdmehe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vmzaitmx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pdyjhcmt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3cvttkgoj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ukzrcxxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txmgehjv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3cqppjeij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iybcnqar.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vfcugwsi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjgnpuyi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wcgtwutj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vegkgfjh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fqsjjqis.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3cnvvuhdr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3slbzzuwb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3aopnczcv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gpizivih.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3hdqeqbxq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3abqscdba.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vsrajptf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ruhdekfl.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3lotxaozv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3jibmsuyd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ubyljdpw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3otqtaidn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3augbwmnd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ejjpsbio.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3akczuptv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ocycyxmr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gkorysog.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3asrkelet.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3hpbpounh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3tssfjdui.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sisnswck.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3uknmfztf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vrefzzyk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvezwvqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3gfejtowt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kzffenjw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rvmorbfq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jqtyxjem.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mopsaolk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nfrexcag.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fgsivesi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3dnzgwbik.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbxrybz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jgjirpvq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuxrdqq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3djfekpyy.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmejpru.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfzoswwa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wylpbyrx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hzoycjby.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3qxvyautr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gymdxpqz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3afcugpjk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3znbjsimb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ftyecoba.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ozqrklqm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3psisysvi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3kczzmwkc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vxgblema.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xhhlhuts.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3sfikgyxu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zjehfwhb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3tqhjbjph.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3fdnzqggn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3husiykqi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3amviqnfv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3inuhsbry.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3jemqcych.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zllmikvu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3azzzrqrf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3creagciq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fjdrakgb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ydbuwuls.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sfxxoadw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3zpizlcxa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvkhpbk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3uwhooiok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxhupkop.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mdbueyvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjwetham.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lqrkcfaw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3fryxzwpc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vktdbyyp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nsxgeeyk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3resfngoq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fklwqwwf.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3jawzhvas.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3stamzhdr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ywvueonp.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eyjevzhm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rmhwzofg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tbutfggq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3cvprmeov.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3agfqhlmo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3vxztouoq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3bculefdn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rgdggsgp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3nkpypcdx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gzhidzkr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3zelpjybi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3tunofaba.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aehtbppl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aymzjcuh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qchipaic.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cnzdkksy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rydtyhul.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qhkapdjv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3gcbjvmty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3eaimjvzk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qrijhonf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vhmegkae.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qxmbzuhe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ajyndyns.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bocsrdtg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vwovgngr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3sneodwsf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zylygjas.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3mntsjxxv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3buqmikqr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3dmhwkbil.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvzyxcv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3uabogbtn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vgzamixq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3pzlipzaq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3umoerufi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3hophojhb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3kxorukly.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3smqilmko.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3akayhdaa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xdmlnqnt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tbbamrwk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3cgroreei.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3gkqlpzeb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3svotecmg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3wxadngff.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3psmoemuo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3azadjyxj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dmcmzjcy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bcalucyx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmketoxi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3dexzurch.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ltrdgtnj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uteumoyd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3wgpusdle.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3uepgsqgq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3vcybepwt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3hgivwpnf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ulwzmlhw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3qipnbmgo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3yjneznpy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3oxogywra.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3kwksupsw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qibvkmcn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3fipxbakt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3selsgaga.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xzywbapt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3krvyjqby.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3dnegzhxm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kmdfxnji.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3qhjceoyo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3genjrrbm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ragbjtqn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3iguvjqip.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ripyvbru.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aywxnfzw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3avsibbwe.html


<!-- 参考信息 -->