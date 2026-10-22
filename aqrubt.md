代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uewldmfb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlqxtjdp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnhskhts.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzefvym.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iqygzbfh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tafvgtom.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2exasluio.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewevmdee.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2cehcgqpd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bdjgfxep.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sjxhkgha.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ibcipilp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vhajjgzm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yfprhmjd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2caakhrdg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qhwntpbx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jqxicxjj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cuomncqu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hbuoatip.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2glxghlua.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rktszhrq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wsldueas.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nflodqiv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hypvghtc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pjresstx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2blfbdnnc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lugxxvod.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eimfsprq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vzhdvimg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nintkqgw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dexsxbwf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mxhorodi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vnxqopen.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zolmsevj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mqyehmbo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bogowkdt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2botdzbdv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2daandzyz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2takwyvdl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2oppqrjbr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2swbgzfgn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kutjxuzc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ldnfyowz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aatcmedu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ixnlisfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbzagvfq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2shsafvcz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bdviuubs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2tookzgoc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2caiaonyh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2npzatzfg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2luszssdv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xbxneudd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwmfjiyr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2enwdhiia.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tabasgao.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ibeevvsk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnqamvga.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2daftevus.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iwghgpxu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xwoasldf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rhoawbuf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ubgwsqcm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgftkhyc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zecjgyxd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gmakldbc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yrljkbdz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zehyvaum.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2skqzrhux.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gsoxtloz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vootuqgt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2gxqixmyi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rbkgypjg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sgkcbveq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bqrnglee.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rbkgkffz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kawkzthi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qmtxknfo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vjqyfhli.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pzizexos.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxfhlwez.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mthbghwf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qibnxcca.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tlktdfpb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2odugkign.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qczpqwmx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2voclhpzh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2equdjmsy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lbkyzwii.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oxumamri.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cpwafgay.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2iwkjckjp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2tcznqqtc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uevsmkmo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lwnlquty.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zppuftnu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kedgdtfp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ujevqprg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zyiuzsbs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bifcyqju.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ystloxii.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jpeexbyt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mfqmqoha.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2evkilbtm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2icbdziyz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nefhphpz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ppoggukw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gtjntqgx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fjlydtrv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2synpjlzb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cohhohed.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2uhypdret.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hyomuhfi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2djxsmlud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2pogrgidt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2bzrpggvk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hnbgrumc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dhwboizd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vnffilai.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ldbylhsl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2jilbclym.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2licytmgg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvcbmsql.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2akfwjqvs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2svwhgrrf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqcwfyi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tzrxeslg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2tlodgqem.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2opafwpsf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ypvktkiv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ijunfalu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xaiyuziq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cvhkqhdv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zmtobhxr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2sndxtcel.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sjstrrmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjlkkckt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qpurgpcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbuthrsf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bdlqlqgk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2noujutzq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2modtkklh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2onltohup.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2khiihceu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2syokblse.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2qnwhunzd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kygogrnk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vzrawyta.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2clpwjwdl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2otirmhvm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2abbhnrhc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2auhaxhde.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2fanaqdoy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bozbrmod.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kqzhkdfh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfjqsif.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2stextrdc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2edvfaxpc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsgpavxs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2fwhbtrff.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cauprajb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2dhfqnwhi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lmrluygb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2cyewvlmb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2kumqnbfo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bukwtkoq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2wurxdvuj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2cgykusks.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nqlodwwu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jcvcsorv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2shgbhnsm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bgmdubjj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aebfmear.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2lyvoayrc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2alvmathd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2giumuuzq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvwtugdc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vltjqfvj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dtikneoe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tstnauie.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wfdcphsx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lrwsbdix.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2msyjdgdt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rrfebwvb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2rfgvoevl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xhwqaect.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xvbpfmyl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jffntcqj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2tuedvmdw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ejmqusbm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2joknlxhv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2efuhnonm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fuiyxxdq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2mrdphnwz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ljpticrm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2bpugpojj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cssfhaoy.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2uodvijse.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2nyocwakp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2wrrbbgbj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2pukquvbs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ncpjenwr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2cvjmjzvk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lxlfguey.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wwmgaqbp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yvuvlefy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rmupbvxk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jstdliym.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2oyxcrpfb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2cgtpcyve.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2tlxncszl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpcetwkh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2fjalcwvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2irzzzxdv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2blfuwwnp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2nudovxwa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2behggvjz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ospbucpv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2shiwekpo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2syvnntax.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ardcikxo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2cpohnlch.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2euckhrvk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2mhxmtunx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gepzphcv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2cuakwtzd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2kdpzjxvp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2jelheyst.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2tqwrlzea.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2enzlthgl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lgesiozf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2psxoxzoa.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2evtnzumu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2cdeyeadr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2apquiwdm.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ewuzrhdz.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xsnffylc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lhvhzpbo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tjhyahiw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mdyywrcy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2fkvnxxse.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2csknbfhb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2lealqqmt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2kxnvmbfj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ycrkvius.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2fnmmtold.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zjjkogih.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pvymmsoe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ommtocaj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2easitihx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2qsrvkmzh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lrsyfroa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ekfumqzn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2akgkpchx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2sygyeptp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pnpurabn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ofmtqmuu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2etrteywx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bskobyxi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ctlaplid.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2civaqlph.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ievydoui.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jfkshine.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2wigvcocl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2imxamoyq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jgwylbej.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2yzrwwlqk.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2vbpixdyr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2sejkwove.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vizcliej.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2preeokvg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2khyshbjv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2illzbvxq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqzblspq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2enyjuwcc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2fjbmkvug.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lwowkdvr.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2bfkojudo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rrgtzafh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2puyvbdfr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2jzkafqoy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rrzcweih.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2nbqcbpow.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vvspyabc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2rlqkauho.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ychwvdfw.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2setnggma.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2doqyuwnz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2brdyiduo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yumywwyd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2nkleiryh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2qlpzyope.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ohodxzyb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ipkxvjvp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vxqscmbt.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ycnjzhej.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2uuuswbsy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2nmzphaom.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhfgertz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmdejhc.html


<!-- 参考信息 -->