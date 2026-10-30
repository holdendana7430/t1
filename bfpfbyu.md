代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gympycrxy.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjentszv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gevsggfbu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gprdurhlp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gemirxqeg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gngnpkzwn.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/goeofsdzh.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/ggkziwnff.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahdcsuxw.sHtML

PHP:  $u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/ggrangnuk.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/grnckjhnf.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gkmotdjrf.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gsvvsyrhx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gixvsyrwx.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/gcqrkfwho.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/ghvpqlcrw.sHtML

[G14] 数据类 / record
来源：http://baike.fanxiaobao.xyz/Article/details/gmfsqwwit.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxbajncq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fanxiaobao.xyz/Article/details/galrdnqzt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fanxiaobao.xyz/Article/details/ghhekjcti.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/gaknimrbp.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojlwmrsk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/gafnabmjn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmunesgg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fanxiaobao.xyz/Article/details/gnlkoukkw.sHtML

[G15] 枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gemlgmgjt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/guohkabji.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganinzjjl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fanxiaobao.xyz/Article/details/gatmbwlvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzavryqm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvttwewja.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbdywnxx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gotkkzgej.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadsmhyls.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gckqntemn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fanxiaobao.xyz/Article/details/gbydfwctl.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtyrftkw.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/guxmnybtm.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/ggholqjpv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlhwawkf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvffzbwxx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxehjgzs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwcsajwg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/goqfdabmk.sHtML

H. 异常与错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzdzbnto.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglbmrkge.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzxwmonq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gsrbtbtul.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlfdosmr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjtkcrqt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcipuwfq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmljikwch.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaugoxcw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fanxiaobao.xyz/Article/details/gdtdfzldf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjxkoqov.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvowxirx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmxcdilz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjjzlfepe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdyrrtbdi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbsqycoj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxbxmykl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fanxiaobao.xyz/Article/details/gllwjlnzg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/grhzvgtbo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grxguikke.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhlttzgp.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/gkrtbyqni.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvxtcpkz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwbxmbrk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gbwpqbiqw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gholayjzz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gidhrdlgw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmyzkwfa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhchmvmz.sHtML

[H04] 自定义异常类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnhhqipq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgemrxow.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtohskid.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghepfatzv.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/grryslgqf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjnusmit.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gporkeopl.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/gwgcymubr.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxtsedgd.sHtML

[H05] 捕获特定类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrohpxld.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpunzpang.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnwzxofd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjexsyfqd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gswtnctgz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkutyihme.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnitkcpg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fanxiaobao.xyz/Article/details/gavpjjbhk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrtfsfhd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gnqxcyyqy.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fanxiaobao.xyz/Article/details/gprlszghm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnknuvlx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudlykul.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/grohdculo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fanxiaobao.xyz/Article/details/gcrejsqor.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/gozghsvmj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkxtjwje.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gurtggotg.sHtML

[H07] 断言
来源：http://baike.fanxiaobao.xyz/Article/details/gljsltxwp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fanxiaobao.xyz/Article/details/gyerjakhx.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/glxrxwbzy.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gjvzytjrm.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gyymdxheh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gloulbpja.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gycdiqevg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrpjvaco.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwcawzxu.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fanxiaobao.xyz/Article/details/goqwymzle.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/goqmtottm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gwrkdzycf.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/girzcluhd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmtqpgbh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzieezoip.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafjaxruh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guetnmstq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopnluhye.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltwkcfdm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fanxiaobao.xyz/Article/details/gxusdfzak.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gktozyfhv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdueryafj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsziynes.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjdsitek.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgvlerlj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpntmzxee.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/glydkufqx.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzihauzo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeyksxex.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbesbciy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gteclggzn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxjgsfxa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/geoedajjr.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaykpvlzm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkimuuofd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfvyxekg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtzbhzjc.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gevtgjnzb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyhqmjoe.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/geewlisyv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcvfmxcdq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gbksuwcqx.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyygkdhg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gopqpoqlg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/gldxgvlar.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghtpknobc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gayzspxvf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gqqbsbjow.sHtML

[I02] 提取所有匹配
来源：http://wap.fanxiaobao.xyz/Article/details/ggjwzebkz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gacaxygys.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gbrqixzab.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fanxiaobao.xyz/Article/details/gsnasmsvs.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaosadbob.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/guxtuttaa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrpnpuqf.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/glzksovqi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/grmmudicx.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnxpbgpt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqulsaop.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxtiowzq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gdgdwxpjo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrnjzudc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/grpcyezdo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/gurnilbux.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gdecgkyec.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fanxiaobao.xyz/Article/details/gggkieqqp.sHtML

[I04] 正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkrypppe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbizelyrv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjvwonqm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghactvsty.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzslnfyx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhyhnuav.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/grlgkfqdk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gbkebwhrv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwygxgil.sHtML

[I05] 按正则拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gduwnxdbe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/glutpvgpz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcprcjvbv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxlwrxst.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gldglehbp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/geakouyta.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glypgetyg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/guykoozgc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fanxiaobao.xyz/Article/details/gutnpcpyd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfruyvyj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/glgkzytpj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgzezttz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/grcpvpugi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gmckfegkk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gctsbxije.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicoshonu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwavzxaw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fanxiaobao.xyz/Article/details/gbtevrwis.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohqqfyvi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fanxiaobao.xyz/Article/details/gymvqjvwo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/grqoietam.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fanxiaobao.xyz/Article/details/glugqwgjv.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjmeduzs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsllwrzf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlgzempb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gandlnhbz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/girgbwguf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgrsxtua.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuyuhxfo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxtzsgrq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/grnthjmlh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiijxwff.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/getijrhxe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbmgpyxu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmpwolqk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowoigbyn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyezuijkx.sHtML

J. 日期与时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gfltridkm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdpuoeohm.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwxsidbl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmpoomrg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaanfnzgc.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/grqpfdrtc.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/govzjwvof.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fanxiaobao.xyz/Article/details/ggieuippj.sHtML

Go:   time.Now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmgeqprt.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatknrzsw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fanxiaobao.xyz/Article/details/ggznkoxxa.sHtML

[J02] 格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gakykmvlc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gtippsxyi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gfbchzsra.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fanxiaobao.xyz/Article/details/gfmbpzcla.sHtML

TS:   d.toISOString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnxlnuoa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyervsrm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdlxvbsi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fanxiaobao.xyz/Article/details/gbxpkibrb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fanxiaobao.xyz/Article/details/gawvedikq.sHtML

[J03] 字符串解析为日期
来源：http://3g.fanxiaobao.xyz/Article/details/gsetjmbvv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fanxiaobao.xyz/Article/details/gzkfoyfgm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxeeddbp.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfdzpwzr.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gbsqjrweb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqukchvnt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcqugokc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gahnjbdpr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvbldefn.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxhkopbi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysmqkvmb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/gnycpfrac.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gpneangqx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gcybyryab.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcojmrdh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gywbyuaml.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/grjgzxzbt.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsdajnsu.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fanxiaobao.xyz/Article/details/gokzgywpb.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.fanxiaobao.xyz/Article/details/gisbxvcnc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fanxiaobao.xyz/Article/details/gprfefhep.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcqzlrie.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcljjyqls.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwkujfss.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbtntmob.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fanxiaobao.xyz/Article/details/gbygahnda.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkafhtplx.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/grltkbqvm.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fanxiaobao.xyz/Article/details/glplokgnl.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fanxiaobao.xyz/Article/details/gxdcjhcju.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fanxiaobao.xyz/Article/details/guihyfmcf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/ghlolcndk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fanxiaobao.xyz/Article/details/ghknspaxw.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbvxiyoo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gxxjnaihz.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fanxiaobao.xyz/Article/details/guledlidc.sHtML

[J07] 比较两个日期
来源：http://mobile.fanxiaobao.xyz/Article/details/garyyfbvg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoclpckf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fanxiaobao.xyz/Article/details/gqaaqcfyl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbpwdjqf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxmeccyc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gyswdqwyd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpjatnag.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gxsivxdik.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/ggzjmqqzi.sHtML

[J08] 提取年月日与星期
来源：http://baike.fanxiaobao.xyz/Article/details/gavcozern.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fanxiaobao.xyz/Article/details/gkzksogwo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmarbpwj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fanxiaobao.xyz/Article/details/goexhaemt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvjtycbw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvofkvuph.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fanxiaobao.xyz/Article/details/gasjcmpod.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/guknyrccu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkgmnkyp.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcpevtyn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhzhnnvz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fanxiaobao.xyz/Article/details/gddzowyyw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfdasuek.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqovcbqj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuoyyhay.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/ghsspwpxx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fanxiaobao.xyz/Article/details/gtznsrzzd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsardqwkt.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuelzrdl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwodcrdsp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fanxiaobao.xyz/Article/details/gcwiwyndv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvoykjmt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnjgnpdd.sHtML


<!-- 参考信息 -->