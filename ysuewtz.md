代发 wailian999

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdqahpct.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdyctqyn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvnazzmt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gizanwkhl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfbrvomu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqzvjgzmc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fanxiaobao.xyz/Article/details/glacaaicp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjjtctnw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gyqipjmlj.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gapwbhnph.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gmdfymzdu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfdmgepi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/guvesieqz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/ggrscmnvk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmphihns.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/gvszxoanz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fanxiaobao.xyz/Article/details/gfryyvbla.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/giluoouaa.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/gseiyteyv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/gysarjyls.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjpmefuf.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goozlgpoo.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gcmpyerca.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyclredjz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fanxiaobao.xyz/Article/details/ghkiececc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfifuqrhc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmwmmbdl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcjdrmuvt.sHtML

H. 异常与错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghckaqpcg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvdyihuz.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/goosvyxzt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fanxiaobao.xyz/Article/details/ghkifryad.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgznuylg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgnjglhe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnrezuiop.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsrahtdy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmjwflyt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcrosmnld.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxsreyuh.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfhzykyv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbupakpr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdbpcafk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggymjqsig.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtveqvtdj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmnywxdxz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhnsohkr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqazbfjuw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqkaftzd.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gpnpojwdq.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gqcorbzjo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmjgyvat.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwdvogel.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtaqcfat.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gicqwhetm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtihcbqja.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfopogany.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnyhzkuw.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlnaejgr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwezlfgp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxbuuxzm.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gphrpbyqq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzubljldw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gadtlbqeg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/gkrvetony.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbtygpqn.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpjdrbhb.sHtML

[H05] 捕获特定类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxqnbbxh.sHtML

Py:   except ValueError as e:
来源：http://blog.fanxiaobao.xyz/Article/details/geqyjabpq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvcgatgz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkcvktpem.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gviahably.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzycrhqj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwwkauev.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fanxiaobao.xyz/Article/details/gxhgzyzzm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzwyeoxmu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoiyimfb.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwpuzuhl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gizhchbbz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuybaqyb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gvgikflia.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtrposdu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzvnaafco.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gheoazisi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoajsinz.sHtML

[H07] 断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpeosvpt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhcykmdj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmehdpsa.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjyvuror.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gtwtosjuk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/gfwahgeyp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaapdeqo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoarztjg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzmorddk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fanxiaobao.xyz/Article/details/glnsyypmd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gtqaxzqzo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/glrmwdhoo.sHtML

JS:   e.message;  e.stack
来源：http://3g.fanxiaobao.xyz/Article/details/gwanluwwb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gysrtzclx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gmkixgidb.sHtML

Go:   err.Error()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjflyldt.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/gqpikbbub.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fanxiaobao.xyz/Article/details/goovpveah.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokezykti.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsmhhvgz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnacdgwu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvueapko.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggelpveoa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fanxiaobao.xyz/Article/details/gevbiwgiw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtdnyupg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fanxiaobao.xyz/Article/details/gngcdrwpr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgcuyqqo.sHtML

[H10] 资源自动释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsspuqkj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqyubfkj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpkcrkay.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gxvnjfngz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gsfbqcptk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzfemizx.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/gvwmdmbsn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbackscpw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gbdaarrbm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvimnezxb.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvplwjoe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhrctfw.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvdqysyz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxppxctyn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gmsxciedl.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gvvqrhfwr.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghjrudnjt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fanxiaobao.xyz/Article/details/goltajcng.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnsomzwjc.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gzivlzosh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/gtigwnkqt.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqehkwlbv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gsjrvbopv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemgakxys.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/gdehpnazb.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gmugqlanr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhvthjes.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrcudnlj.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/grpoegdow.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmipmsdj.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxurtaldr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtrlprjvr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/glonfkxmo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gqtlaljve.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gteenyuye.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gigewbpgi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamxmekqm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqluoyxr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/gsmvjixdn.sHtML

[I04] 正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpmnhzvt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtksvgfnf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoyhtzoy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/grvbbrndj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gzxfsrcej.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/grgzgoirh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gyzgorubs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbbkpznq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/givdhgbzt.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluwlpqka.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpbtnelq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmlxmteq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpowffyl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwbvwamc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/girdycnfs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtawgkcal.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgogvwsc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/genrthiqq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fanxiaobao.xyz/Article/details/grfclqhhu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrbdpuya.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/gttjsqmes.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaelbgbt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gkleszkpa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gzwtxyasp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/gxytegcxd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gtorqiwke.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gwmpljtki.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gobwmnexl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fanxiaobao.xyz/Article/details/glltzujzy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gmybxkpum.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfooghmr.sHtML

TS:   /error/gim
来源：http://baike.fanxiaobao.xyz/Article/details/gzlnhbbzx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/gaddanorf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fanxiaobao.xyz/Article/details/gohwebesa.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fanxiaobao.xyz/Article/details/gsbzroykl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtavmgoux.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gynpgkzmt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fanxiaobao.xyz/Article/details/gunqjeomg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/ghgubboub.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gdtwexghx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfbihbrb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/gtbzocmgi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/giblbypwl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsjsstwk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtvjcxpk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gotxgkdat.sHtML

J. 日期与时间
来源：http://baike.fanxiaobao.xyz/Article/details/ganrqseun.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjdvcoqy.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfgwtpal.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fanxiaobao.xyz/Article/details/grvfaavlh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzgivalt.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjqaact.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/glebeewsk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfrumesi.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/gyeodmqqj.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/glwqykqtf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gciknlcds.sHtML

[J02] 格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiiterak.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcprotar.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbgymvif.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmdiqvuj.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqbgphnc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/gbzfraile.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fanxiaobao.xyz/Article/details/gjmiwsowv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gddqqalcw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godzxrjam.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuoynwlt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjcdungl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbbuiyxd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gghrpzikg.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzigvyhrl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gykghbfli.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjbrlxkz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkptybxv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fanxiaobao.xyz/Article/details/gocrencqp.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/gaxnuwkbo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzkcpkot.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfdacdpj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gnikpboju.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvxuzysk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilwkcrlg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypooqbqm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/geunxbaox.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gavpcqvyc.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxnxzoor.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fanxiaobao.xyz/Article/details/gxntcdtre.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gbtjaymxr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gopotojvj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnhzhqrw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gkwhewivd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gptutiwaf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.fanxiaobao.xyz/Article/details/gtngjejlc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fanxiaobao.xyz/Article/details/gwftbpbpw.sHtML

[J06] 计算两时间之差
来源：http://read.share.fanxiaobao.xyz/Article/details/goljeficn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.fanxiaobao.xyz/Article/details/gglmpyjoo.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmpbvejk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvfhzyud.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fanxiaobao.xyz/Article/details/gfxpsbktc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfxtlktq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywnoazbm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygstnjrg.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcclcxap.sHtML

[J07] 比较两个日期
来源：http://mobile.fanxiaobao.xyz/Article/details/glyowgudo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gbczqvcfs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphfzclji.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gelyopstv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdvutewr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgzstxya.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqoxiihg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gudkwvuaj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/givjlgorg.sHtML

[J08] 提取年月日与星期
来源：http://blog.fanxiaobao.xyz/Article/details/gmajzvyos.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fanxiaobao.xyz/Article/details/gfygqryqs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxpujgtq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfbptiia.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdvlrcgd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/grivjfgpr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmtxmmts.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/gybpkiswp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpqdzeup.sHtML

[J09] 时区处理
来源：http://baike.fanxiaobao.xyz/Article/details/gjkzhjznf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fanxiaobao.xyz/Article/details/gzibnqnqy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrmkwipy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/giodchzds.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifklctyh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuboznrs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjlroxwl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkyoyumy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/gjabxqoyj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fanxiaobao.xyz/Article/details/gcablaxve.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxxxgwmv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fanxiaobao.xyz/Article/details/gpnhumkqy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdnddtiu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnivvyrd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnrqpofyo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/gatcargne.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/glgxmazzc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxkdpotf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gysifwnfc.sHtML

K. JSON 与序列化
来源：http://m.share.fanxiaobao.xyz/Article/details/gubxawfxy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqhwlyme.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyihbogt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/ghkedfxmb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggybenspy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmdmgyts.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gppfqdxzk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fanxiaobao.xyz/Article/details/gblwpebqs.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gatkxybxx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fanxiaobao.xyz/Article/details/gilhgrncz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkskybhc.sHtML


<!-- 参考信息 -->