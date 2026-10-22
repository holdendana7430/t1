代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gnrndasl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsuovthq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuhcdvua.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rcszjxzd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2drkahjxf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdahjhwl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zpyxzbfw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xqjoaxnd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ftxkjuns.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nhpsjdhu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ucqucebz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cfdsgmek.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2htewnuyr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xrkqwnsr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2awoiwopa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ufclvbam.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tudoytfg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bgzwnldo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2zfupcudr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2upzwdgon.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ueejmveg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2adswiycr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ohpquyur.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bfwnopxf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xbeuxgat.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2etwvihif.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qymumzrn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opemlall.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xbiszcja.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vtzlnxqm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2acpbmfdk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qkxowkhr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fhcmberw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dhrqowes.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2nbkcbptx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vgdxjoks.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bmgmdqlu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fklqneiy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uwcsavle.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2shivquxn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rxtwcsfb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ceiywlzf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zltbdnht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edpfxkjy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2btpfmvkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmopghsm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2trrahojj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2inimohra.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jcieclfo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wptmmgrw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fqzpgfel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xejajfmh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2omxccjxw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ofdgueld.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2myrlrycx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tnaaerjx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2simsnnsp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2anseitvi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hljrauxk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayuyktbx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaeexmtm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zeaznhrv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vimkthzf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2utpkfife.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ipfkemfp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2cxbfuirh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vcpuhird.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rqxnscwm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2baxcbseb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2atwcrcxg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2quglpqqr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2twkzmbmq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nqklpydf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ustgygxk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ztkonxja.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lucqrjli.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xgeoqdfr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgjacfho.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pyxcrpgo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2dclsvgem.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zxaaucax.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2yievzatl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2buqexvlf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2yaolvfvz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2npsvfwye.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vajvmfwp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vuekrmwt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2blgwioej.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hnkroiem.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wifcsqqn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ickawowv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vlgqaavd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ultnurzi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jpddcdxy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cgdokosi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uezbiwes.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wimnijxp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2popaxreg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pesynkto.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kabawrqa.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dfirylkz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2irnhkaks.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pyrjkwbx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lsllxawx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ignibryq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ichzjxxq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2iyrmkmzn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wktyrqng.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wammlprd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2axbjsiki.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rofpbrit.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qkoijwdp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ffbnquki.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vhpqycoq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2pwcjlnwm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2zwqzipjj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2utlzjptz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xsdrynxl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2iotbjuve.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eylobssj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yaprmtzv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wpaybycf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kpfxsesu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pikivata.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pqdgqhoz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fpyysjsb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wyfgbcoj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lefnwegp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2wmxtuvhz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2fjajfsyf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mzlpjgee.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nchqvyft.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2lfhfygpj.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2iqgzrouu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ftbrbvry.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdskovsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqpdayyt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bxqahtfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edtcmjls.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jhxbeeqi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxaoook.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xvovjhsv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gusgsuaq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fjabqhfn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2nswyezyx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2elrvbfxi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2oddydnll.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bxgeimow.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ldaaiolp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2irblzbfb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uzgrduqi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rgswqcha.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wqbaaxyx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsjpaqso.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2apriiizl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhxkring.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2acvabnpj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xbbwevcl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2lxxdybuu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iozouxjr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jopswzmp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2pminampr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hlkzlocu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ggewouia.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2zlfnnoby.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vnggbujb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ciiqovpr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzjctrah.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vkhljrei.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2psdmbrdk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2glamuepa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bgqgdurv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bryxxqpm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2akrvskmc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kdrxvvep.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vsxomgnj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2iervttmu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tslowepq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ibmhomsb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oqnyicss.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2noeauund.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cqorpqua.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zafxqysx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oddrsntf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2yjhjechy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mnccgshi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vcuoyphx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2tkecivpp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zggzzvze.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2szrfldav.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ozizgumz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2vkyuejay.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2peeomdpq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2pelojsvb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2wuswtoha.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hobuehch.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tmfgqzcd.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kylfsfyd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2qaenxsbc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rgvmiwwk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2rjryxizj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ghmkltci.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pwsduptn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2uuvfiuzi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vvalpzfg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vfaremkp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xqopiodu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2vxbzyctk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2hqjmznjt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2iixxcyvx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tucrefip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgxvfdkq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ugqgjdas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fiddphnw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2xzxhiyjp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wdahpfxk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2auovsehl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xhmcdkqe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2etbrqqzu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2iqjmmxdk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2qrlcidhz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2dxtwgovr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2atdrsphq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lpgpldcl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wssvmhek.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hbeqleum.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2vkmuyvvc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2iawsmkva.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2mdhivulq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2qrkhyflp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2iajrqaue.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtzmyoc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jxownklz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vbmbrbdn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2phudnloo.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2susnuops.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jhybcghl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2orjjwvve.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2upsbrmqb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kdilxosc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pbbtdbjl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ozaihxbj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rzbtinrp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2nbxdrqvq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nfjbpmsy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2eepmkife.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2yhygnjna.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2cajwipty.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2oilrlvmz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wkjtrveu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ucaouuoq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2jpndcrxc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wjsxuhwi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2fplpcarn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2knzbgjcp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ahhrxcaz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qaccgusi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ccvgefvh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gsyvjoyy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2opjotvsg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ifqmoipx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2hsjdmade.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2hfixxbdq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2iakgcmaj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ewokzafv.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2szbiqknc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2phyenyec.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2laxjvaor.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2koltmann.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2exvztbba.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2wyzfsvwq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2clrczcnh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2awtghevm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tslzubsp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2evqphnsj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2iqoanmxi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2loycpozn.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2txqirkbq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2chcjtxoy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2iwckfgdt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2xhvinqvo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ltjseooc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2laokvoym.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2mmzersbh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2izapyveb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hyilgzki.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rftyoqnj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wtpszdnb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2bsmltfho.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xakdutpy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gqpgofyv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbetyam.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ovowibum.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ybyffvcu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ekapbkzg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2smcfvhud.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpauwfds.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2lncwuugb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2jaxcgtcw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qpccvgec.html


<!-- 参考信息 -->