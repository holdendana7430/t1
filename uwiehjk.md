代发 wailian999

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmtkipfpi.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gjqtexptx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfckdtjfw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/glgyggwgb.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gergbwvql.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/grkhbpkca.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gwpgwpkpl.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghgtcfyuj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gtteurzog.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gbkxbzpmb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gasjlslqx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnokfaost.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gzjlwbgvy.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/goaphznps.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gevizsdhx.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gaifyatmr.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gfwyxwdsx.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gnqugwuwb.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/goqiaearm.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwforjqtv.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gyxlcqvcb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gfpfyyspd.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gkyapcpjc.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gozxntlep.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/giuqvvurd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gjcjfbpnd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gkkiyruqb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gdrgnrbbf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gamziaxil.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gzcykvmgt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/grxipzkil.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gjwyrkhla.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gzyawzzrs.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gekhdsppx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gxfjfjybz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/ghbcnvxkk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gxdnjepsc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gupglfaaq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gzzduiftl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gzhpbgopj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gpgbebtvr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gwbuuppsy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gdjszktlx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/glrtxkrhg.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gvctksxpp.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gwynowzuz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/goiqchhxq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gncrhqqmg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gqspmizys.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gzojcmidd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gdziygjjh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqwvpnhcp.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gvgbjzqms.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnygtudpq.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/goqocknyu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/goozkknem.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/ggyaujuws.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gtmrxixif.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gvzebbrcm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gjvvgwlnp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gkrpmudcx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gnhnauqqt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gwaklleoy.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/glmcumenz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gqaedisys.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/guigrsiap.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghiyvebro.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlenanze.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gvhmsnsxs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gvlqvnldg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gshdvhacn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdorvazxm.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/ggsbcuyrf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gtlahukzh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gkucvjtlt.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/ghekmrjps.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gkplagnjn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gibjzfwsv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gffluvhdz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gwtzzzjao.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gddxxomsj.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gexpvqgmm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/genewkheg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gcirmhket.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gxzdkwhii.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gtpqlodlw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gdedgzfqv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gaqolmncp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/glueouyzp.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/ghlosuoua.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gxzdvaxca.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gufjjjqiq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gqepfqbxl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gwolxiias.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gruigtwtq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gclhmkbvr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gjrlmqzwe.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gtikgtzbp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/goqutbhlm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gzelyjlmh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gbloiehwi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gdsqkbvpm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/golxjysnz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gumoltjzx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gkfuwotrb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/ggdocndzv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/glzfsufvp.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gzcpxqllh.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/grqwtoehl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gduhobgxl.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/guowlxamh.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsynthrqk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/goaihxppk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gtengxbnh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gmpfqhgtb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gbvzmdqtj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gxrvyoibj.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gmrzecnfb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/giuvuotdf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gysavumgh.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/glrymzisq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gwotqyhrp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gzlhgmdch.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gthihzkpi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/grmagllhi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/ghwqeuxfq.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gfsqwzvyy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gyzhgsrlz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gqcycpzjo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gcymvrcew.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/giymacapr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gwgncifls.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/geqycrhbv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gflwgzmym.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gtbmqzilq.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gwzkaqbhw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gnriquvmb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gozwewzqh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gkepzpftc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gwvdojxmi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gvxozygoi.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/giziukopm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gnfedboxd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwvdullci.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gholzoklj.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gihglnnzd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gswmxcfsm.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/ghowrvkyq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/glqlnwpok.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gniagufoa.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gjmrnjqoc.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gczlmrhwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gldkdlljx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gagsupcug.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gdgbxpljc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gfrjtpulo.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/ghalqdide.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gaftveigr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gyxuaxigw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gsxqakico.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gikytufol.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gjnvjilnp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzabnovfs.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gecxsfdmx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gphoacorq.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/ggduyquxu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdsomoq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gskokuzqv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gvfdhvafj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gaiheutwt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/geyyhwtcb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/ghnjhjbaz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gooijywjk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gymknogvj.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gmfzwmzwj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gpiclpign.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gyloodnjw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/grhkfoymu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gpawretjq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gobhybmnw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gyinmehtb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gpieinako.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gackzsbsm.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gttdqaufb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/ggeayaqpw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/grjrjcuod.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/grejipzvc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gpeshmyvh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/grwpthcbp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gsdlqchmh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gnchdfykb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/giaxlkema.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gpesywcma.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/giuomkozd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gheusuihs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gfubvkawf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gdsixpsfv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/geetsqjee.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gbtwnyhlu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gndtqheiw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gdszporcr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gresjevrb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gjuunhbcz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gbstlxvpx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gexjtatmk.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gcrtrlqse.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gwgeypfwb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqtelwu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbadgifbg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gahvyjvjf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gwcinmjdx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gpbafwhxr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/ggakveacf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gudcgkpus.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gfqbvpnsy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gdyueglac.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gspxvrdfg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gdkhoyxas.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gloprjmrq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfsklnnjh.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/gehgdynbp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjjurgyul.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gjkolgxta.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gyhdjtgqs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gvhwyzwah.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gpuuftacu.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gkctkslnh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/ganytowwl.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gnefjhzbo.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/givcurepu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gfklzsgjm.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/ggbeaobxm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gzbfwosft.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gnyrgaots.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gjhxkynoo.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/geiadhxmx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/grddtkavo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gxlrfcwoi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/ggfttcxtu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gerwsttva.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gdzouqhmj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/ghorkdvlf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/glvskaoxn.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gcbixpzpe.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gagcowkjq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gvhengsrw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gynoajjni.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ggtyqcsnn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gtctswmxf.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gdftaipnb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gozrvspzj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gtafvawha.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gatzgljzo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/goczvmgvx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gbeyplxtv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gzkdfjrmt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/grocipjuo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gtzrsgsth.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gxuiovteh.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gztmrjrzb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gqcdtqhqe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gztxqbfsg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gvvfgebza.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gsckgjksh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gmamfjivw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.zdbjq.cn/Article/details/gkmpohdmo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gbraadajo.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gfztoftau.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gxvdefaoj.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gunwuibib.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gafsonxnv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/ggkrypxvf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gbsfqjmte.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/ghbedafvb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.hesvh.cn/Article/details/gzcgqaxrz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gwjciqmxd.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gobtmrpsp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gnsxutpad.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gclnznjnb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gklzywarf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gzgtriasp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gjokmtuue.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/glzxukkxh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gokheehgn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gyyfvlogj.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gjxiwmcax.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gxchnowry.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gazapccjg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gunzpfros.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gnofeydsp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gschbtzvk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwopmfn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/ggzqthmon.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.hesvh.cn/Article/details/gvtmndsly.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gbvnwdgky.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gpxpjepwn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gikpmlbhx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gwszxcquy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gahbdqbmt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gnfhawxcc.sHtML


<!-- 参考信息 -->