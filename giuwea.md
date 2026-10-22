代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqkrtazt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpdhwmuf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzuyrbna.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnhqmgf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ncqvwsts.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tfncxtvb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mdjtibwc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tslycfmb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hqtfuwge.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yxgubnlz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jqwanzia.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xlvwjcrs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2chhqvghl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qmrsqqfb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rnsepigf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ypynwszw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hzapocsy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pvntmcnr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hbllbgdl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nqgzrqxk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jfmcalyd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehurnmnv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yaslxoza.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2eiahmyov.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2crmumfyj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2emiiwexv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zhzgmvdp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2aiwuaabw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2afkaxufe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zxhxphgx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zkatokwz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mliuuuhu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iwkozwat.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jzmbcthc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wxoovvsg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2fyeijuut.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2lqogijai.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjdmeth.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nmhgaadn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zrjqlwkr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2attmupvb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2howbwqgt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qeffosdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izeskrqo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ekwnmqva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwfhezmp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mqlcoulc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kylxgqgf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxitrijy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uazqcemj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqgfkvkx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2yisgyqmt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wvozkrpd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mshucjer.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnwrayuj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nkoaaupl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nrzonyoq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyztpafx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xprxxtus.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jjdlkjmm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kduluofa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qrlkwzvh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dqbqbrdr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sulclcli.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vhcvbrtu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ggqxnusn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mjaonvof.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2afsozybb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pddcngee.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mdtkipgk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ecyslkyc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pporvubk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ahsfstdt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qvwbpmap.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ulzwhbhp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ukwswxdl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tmsrofdy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqfylwds.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2arrowzdg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wjndzurr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lwslocly.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qufwzzgx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kxrfbcgb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ubzbffsq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2eozlqmyr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pcflhfof.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlogfyxi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqhufsxe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hkrmyfyt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mjiknvkn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2okrcclqz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zhknshfs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hdxccbwo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ljictssb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2agasqjvw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uyqmhejn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2clvfjvbl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2juxeevdl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dxkriikr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qgrzgmez.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hhfhjznx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2niksyvkk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vrzaqlcx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mfttrgkf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hnoblfzv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vpepdfyy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2adtcfcah.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2etiusatw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kwnebjzw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2axykhbkw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lfhmulgh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nloyvali.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qthlazuu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqxyhlp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ggelxfoy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2pnabynnn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2bmbnicrd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2gfdkvfuv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qofighbg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2olljwphw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kkafmfet.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nmabmjtx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2frsybovu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2arhitiwl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tlbwfpdi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jporfzxv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qakdbzjw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ikjbgvqp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qwigioac.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2fkmsborw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pdypwlpn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cnpbuyxi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2baukfzib.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zqzlazfm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dbsgfgss.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dlbvxthz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkqpiqfi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2pnkdnqec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvtliqeo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2kqxoovde.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2awxnecjo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xeaxuonn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cwkodhwi.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxnmbiop.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fdvfueih.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mltvcbdp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vsgupyxt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rfdwhvjp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2sqavcfua.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2blvpyied.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2silfmdqf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vtmkldqs.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkfaxgl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ypprhfvz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vgcjhckw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2paynkttf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwvlesdv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2csqvauio.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2tgkrshqp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2roreedxe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lcxadadr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2iypdygwz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nusenidp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2yshjszna.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nwmfhldt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jgczobkv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2arnrzclx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bbuigoow.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yfvmvwgm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vrteolee.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xbxfxroy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mjqjkbew.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wcdruqdv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lphnwfwj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nkvwvkzf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vimoztrp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2qewhndzi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sijtrdls.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcckabd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kmfregjg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qibklopz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2scfccayr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nfifofek.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2abgadhrx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lxoskruf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vvwlampp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2lshdphck.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2akhxkmgn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tornthwh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jmwodtpm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2xiatomth.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2eiauzfoh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hzttfkyo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2cjjfsbcf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhkffws.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ibvdcmzy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qjfqacwp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2dhhtltiz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tftfpjrl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2mtwxityz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2uunwsjtw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2oktktmyo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fpisgbrf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gcsubxsq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qbibpjui.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mwsojbic.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zkowjviu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2oztqftze.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2jdrhxktb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2rieniokb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dnjzawor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcfwxzls.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nexrgxmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwnkorlt.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rynfcqhe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dzqlfiwm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zjprymnh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dcnjgejb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2sjinmxsw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tfhwzebq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ciowvfwf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2ewwdouwk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2rcxixkyc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ganqnlgx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2iigvviam.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ottpgysk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2pblifmdd.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2bqfoeuzi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ogkhxqhf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2lmjzqcnf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2onsvcpnr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2incbehqg.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2pfncclgf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wopxdylg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2gmjwtsyw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lmtxpgtn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vymxtzcv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pdgyliie.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2isenkfdg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xjsvozcv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2wjptvhqu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2oxsbhsnn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2cnnltmnb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2comefsxy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2pghrkhmf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2yjtxtyaf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2louqsgjd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2uorlnpxk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2kgksfhmx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdlpeih.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mxytorzb.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2sxesfdnt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ycloyclb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tvgqsjby.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lwyspmup.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2byjfkwaq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxsbbaf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ogpaamlz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qipjogtd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2tmzuxqlk.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2iefqjbmy.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2qqqzbayn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jafjfczs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2sdazcbiq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2zcqujpkp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jfcdhivo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wlbqqife.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ixtqejlp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xzerqvhc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ygpweggu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ppbfxbaq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kzfbjtjz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lmdxfzgk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tkgruybl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2umdhwfne.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kgumuobp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rqmfqvdi.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2kdxpoekr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2qwdksawt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2zuippuls.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hrkmxbdc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2tagtclgu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2rsxabcwi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hkpjmlkw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2oiholbov.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2rquksfzi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2odvmwgof.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2mbggmkav.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2xzfhevht.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iuwjdyir.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2dghirumn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2lghgcsow.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2qrvvagsh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2gezjgcgv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2wcpsiuxj.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2qfpnhvzg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tkiustya.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2czesngho.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwnbffa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ljkaaxir.html


<!-- 参考信息 -->