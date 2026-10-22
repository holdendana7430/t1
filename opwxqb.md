代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lkhplghe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxlkxnwp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ifamskiq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hclworqd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hbebnipd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ahdnstjj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qtszapxy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2flfzfcjo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qsigswsr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ajdhmqof.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jvgezasz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2abegseus.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zbamdamn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ylustcod.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dqeqmrwm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rdpuwxvq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nalbhopw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zhzdxtrt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2szhxmzlk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lpkgvbfg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gptgalgq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlhrwklc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ibuidjcn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vixbliro.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2flfeaixu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ntpmbazb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vzhxupfn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogqwjsof.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zqscopxv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fgamwcvj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ossvjxeo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hhzxqhvy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uyegimmw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ctqzuyxv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vbjbtlpr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wfucnihf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fejjiymm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nvkxzcsc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wgazeofl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ukeqincz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hvnycahp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2blycmlnh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rotzntku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oarxjuzf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nsgbvzic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtnkucfx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hetrmfaf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kblkkrja.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xskzqgad.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zyebrera.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xumxtvrd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtsehapf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cygjqzdm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2whdsbjzm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkzybogi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2spxngfqu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2caqoaqey.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jplscxzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdvrzuns.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmnazvhb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mvftagtt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2dvnsenir.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrsexxgi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ptkwgemi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nladqzzu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxnokej.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2olumwwct.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aycgyunx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ubwjtejn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ytlbpnzy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2mfqslqcy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2afggrwqp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2scsmldar.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2opjjrdns.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2isxjzyih.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wrdibwut.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpbdtudo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cghxccig.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijobkmst.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jbkowgne.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2llekmtvc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bazrdqhi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2viaiybto.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2piyzbgbi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2khxtbsev.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omnmjlyv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxhzhjdf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ksozthzu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2dmwavujr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2stcymzyq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sicwjowa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ayytnmed.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pbpgbwez.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sghovwts.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qxejmtwv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rdpsxlbu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2fxxcwfib.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2iekzhuxi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ephstzga.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2sxqfsuxk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kgjbndyu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qjnjlarh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wuifzpqt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2srpnggra.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sylgtdun.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2okdulvfp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rgpwpbgu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qtmynfgz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rleqfpla.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2eeewditk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2niapaumf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mqibubly.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vbplelii.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2obqbplgd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hvvglpih.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bbqukwmo.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gswfcjvp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2udbkgmfr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jpubsgpf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vdqidhyl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2uqbizrzr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ezthggep.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2aiicuoqa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2oielyykb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pnfpgefg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2cugyxgrc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2yplqgorv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2elrlqpwc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2yvyvsbnk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qizrclcu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2opwkzoma.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bxpalimw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2nopzkpqt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mduaxriy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xguchahe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2epwtinkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibfnmcrz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2twvrnnao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whqvjwqf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2eyndoinw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xafkyiac.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixenthjo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecwuxrod.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsurdij.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zicvcnvy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uniucwpt.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wmkfcccf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fqkpkgev.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2yyedkhlo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ecsfckes.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2qiffrkie.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2pezbgdwn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2webljhbl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mqaypeii.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ueeieocl.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gezlisxb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2khtonzhh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2aneeztpi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zerokssd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2acjpbvnx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wxqdlsrs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ggqbjgil.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2bkmllwrj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zomxeeai.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2kxtsnqof.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2zvkanqqo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zkxedjhb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2lkeupxsu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zxjouzuv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ciuirdot.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zxwknskp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wbbefhir.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2prulmuxs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gkhwklpc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ucilcehj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pfbgqgfn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xqoynhsp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zhnmoyxe.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oojvoskz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wrftmjns.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2klvnctex.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wrhfhzht.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qdkedmte.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hkrvhtpl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ikimoyyi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xepsvzab.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ydvlpvxr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mwsenwbn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jzzydjhd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yzlgypob.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ltsmjpgg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2fzbgbpff.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zwgxqysy.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kkawbipx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zqpnpfny.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2svkxdxzk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cvmpeerb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2twedwtfy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ufibuqow.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2nirvahel.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2fwbznrve.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rvonymmd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2prqezxjl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2phxvwzyt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2yxzwwrxn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2szqrmckn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wivklzno.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nbjtiplu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2dljnylrs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2iquweeuy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2dggrzmjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjccmhbi.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2rfecbeox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkpaqjbh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2bwecggcj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2kismgxhx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mptylcoo.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cbnmvnpw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hxnxoqmy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2okphkoja.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cchbwcsc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2icszfotk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sgdialpy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rdjxapor.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jcvqntmx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ohyjuwtq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2uqwqydbc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2alvfretm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ojtgrjyw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2mesrxitn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2uzlnzobo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2emmerjib.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2dvghodww.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2xqbccsfx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2kukngxxg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dxljhlpr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hxhcontl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xmcgyxcf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bzlacfxb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yvwrqfcb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2goztsgex.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2anqsfuas.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qlebxjcd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2sevuwobq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ifrogggu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2pnoamwyl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zmqvzcau.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fwjdfcpx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2fzxrnsul.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lcaxyctb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2bpvrwsrx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2gbvsdihc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2fxanugbr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ujssiinz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2klvugtvt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2trxfktpz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qidjrdnt.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2rjzvropr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bzeivxui.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2deypbkvp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2iilhilue.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2bkdwfrwg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2huyltjra.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ydbtkxwn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ogryhfjs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2roizztwf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2auzvvofc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2tqljdvwa.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2svlhyiwr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2eppijfel.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ndbsnghn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2namakhrk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qeapqcjx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2janfdnhc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwfuioft.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2sgayuczy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fudyvghj.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2adzgpvum.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2zjmqgtdi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kupcgafk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2pakzgmoh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2ncdpkcfs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2aneaccvy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2kggbfunn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2nyzaaucu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2tepomdgu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2eldnngee.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2bikiaspg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jratffpr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vehdczal.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jddydhhj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2arcldgar.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2phhgbxno.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2uurjtxwp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2poylprfp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ohraopxh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2daakyyyj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2flzpbivp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgpybwhe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lmfmdare.html


<!-- 参考信息 -->