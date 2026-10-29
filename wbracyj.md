代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gsacilqoo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gboshmrlj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ggebaaujb.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gqktxpgnj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gkbozihxe.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/guwlkjbql.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gwaeioxef.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gdcmahtyi.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gvpngovqb.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gqntjyaqu.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gebonbqlw.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gillhgsjf.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gzjnairic.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gohzdvlbj.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gwkzpnggt.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gvpjfgqxe.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gbgwwlywd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gygtmrass.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gbxmehici.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gajjgdeco.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gtejzofro.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gdmazkrzb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/goxhznhmg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gspaqcdtf.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/glwqwvpvl.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/ggnuoubtd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gzlkfjywq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gkldzgtih.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gcvagueyv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gomatcggy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gvgpncwon.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gtqjoxchs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gfqhrlhwj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/godxyoxkf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gyndlwfsh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gacavncna.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gkfwqaltf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gvcjglfjp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqktahyxg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gelrpiwos.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gnijdaxyb.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gyrzevpaz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghycnfkhm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmgekabon.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/ganuqnabl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goowglrhl.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gppedyslk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gajyavriz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gvqdbahys.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ganjczswk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gafabslvx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gztyzupdy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gdumdlfxj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gtpitfyvo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/ginzwjxzw.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gggwyjlgm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gzhaijvbm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ggnnidkyl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gcescvtls.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gsgxklehc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/geqphsvbl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gpotnhibn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gqtxirusr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxlrvoazw.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gwaxkkchx.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gczthgctm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtnddyana.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gtmqviahr.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/glzyojbyd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gictgzvfi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/glvnudmbr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gdpuuarre.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmzybgyxb.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gdowrkkjy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gmiirvfgk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gtjclcezn.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkrmsgxms.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gwlkctqfy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gtgxwwgnd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/grdjngurk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gbnnstnvx.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gduqsjjse.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gkporazkr.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gpbnkarrt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gcqliaskd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gbcaeqrld.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gzuoickys.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/giijvulrj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/glhfebqrf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gcaapabqi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gvklhfulm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gmzrvpfhp.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gxgisbpzg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/geuzrzxqy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gvgvgcrws.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gavccfddt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/ghevwmjdl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gfyhlnepg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gzumvppcu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gpykurqse.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gnzekjfea.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gzdrjdomy.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gbfhmpvtt.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gnarqtohm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gpvlitfem.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gcjisjemz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gonrqpfzo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gxifvxfya.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gyodeykwf.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/ghmtggsnr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/grasqzmfo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gzwoqexrz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gteenkndk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gkecssdgr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gkrxhjhmv.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gntbtwrbv.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gnyhrwpzz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gwgoqhrrb.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gxrtsynub.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gaxjaumww.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gxlpzajiu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gjfrkakqu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gkmwpounm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/glihlojui.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gajtungyc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gdoytibiv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/geashysun.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gfrldlosu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gwzcyshjz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gmevfvfyd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gaaivvrml.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gwyarrtxd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/glynbbvqr.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/glgosjwkd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gpcgxnktg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsolnclbl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gweqxgvcw.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gspfpfpgh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbejsomjg.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gwynenepz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gfalebyfm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gifagxqyt.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gtyuvvevy.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gyuwehfrp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/genjqrpli.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gqfocjrpb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/geqknedft.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gumnasnun.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gamydnzqm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gvqzgskdd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gclzeqvcs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gcymqykba.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gtpjbdcrd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gtizoduri.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gavasfsdr.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gwqmmcaiy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/ghtkostep.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/geirmdwwe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gukexykws.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gcgmvvbxt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gdnthwcbl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/guhjdthpn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gpuhjixka.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gtdhxevxn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gtgenradh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gfnzaczsv.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gnqshcbwh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/ggfbztcsg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gzzbrsawp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gkwkqayqh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gfklxzmlq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gasfgjwmj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gnfnmgely.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/goopswvol.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdwhapr.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gwznkekla.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjntetb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/ghnwkmtoj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gshdhxotu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gstkldnye.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gabrcitff.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gaaxryhan.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gdtvagwqa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gypqoioks.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gsmvlbfpp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gglxykkjc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gcwwaotgl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/glqtveoqt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gsbdyetdq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gimcwhqxm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gzkyafvot.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/gyjpsmfxu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gmibttsbx.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.hesvh.cn/Article/details/gszdtchuj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gdqjgrbgu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/ganmylfgk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.fehbvm.com/Article/details/gtxufgozx.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gndyxcilr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/ggyzazrzk.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/ggszruxva.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gwfebtnzc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gmbqfuket.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gdtfojbnv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/gsgqktpbh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gwckkivnn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/guwtbtqiy.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/geaxmhqdo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gtfsyeuqr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gphyjguxp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gfxxrywza.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gpvpenzjf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkyxkvjxq.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gvriiayrv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glmtabwem.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/grmfbnlbb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gctxzeegn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gidquobmn.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gcmpgpose.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gencqeyma.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gcsuguddi.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/ghxkfyhco.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/gkbolqklw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gbyfgurym.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gusszkuec.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/glahtyojl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gmfejsdwb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/glidiodoa.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gjjcwifsv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/gtruaxqko.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gdibcaahm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/ggudagqwp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gcywkgnpm.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gwjgidpcm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fehbvm.com/Article/details/gktmocpds.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gdyhtrbab.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gsocrmygq.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gsufrsbjv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gdubldnos.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gewknhfxu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gwowgsafd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gcjflkkow.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gqjlleqav.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/giyduwotf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gbhmkmtox.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/giadtmxle.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gecduoepg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/guqhvukby.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/guvajxxcd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gjvnevain.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gcgizsjat.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.zdbjq.cn/Article/details/geiebregr.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gszibtxnv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gsftawaiz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gvazyuemr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gahbimkgn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gdwtabpnl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gztqmjjwu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gvxlinrrp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gpqsjjqzr.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gltrsgbfk.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gdemptjpj.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gzrvdqcty.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gijcgdhrb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gbzujtbee.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gkgtnhqfz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.zdbjq.cn/Article/details/gtrdlxasa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gmqeipzvr.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gcgfikenj.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gdlyqhyiv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gypqqauqw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/givkspryp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gwdctvvtg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gwgmoqykn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/griybvhew.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/grnbfrdiu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gwbcyjawl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gqacswnzd.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/giywvpehb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gowgqbggc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fehbvm.com/Article/details/gcnhtwyjw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/gfpgupbeh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/gmquwbrkr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/ggjlxqtge.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gkbpqzebn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gfoncmesp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gdedeptws.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/girjlqdsx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gsqcwyvfl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gfjtbmkmi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gaavjiecq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gvdmbjxpn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gcfsdylto.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gnralzpcq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gyfjqvjnl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gzotsbiou.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gmwwbvhli.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gbmsmyitj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gkwathfsf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gwcgeqste.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/glvhnsgun.sHtML


<!-- 参考信息 -->