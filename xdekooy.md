代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gepghdivc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gpjckhpar.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gqpyryqpv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gitxwqcaa.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gewmhfhoy.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gpenvvyqk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gzoffobsm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gppkoedtr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gujfzanji.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gfuhkoedu.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gpzjyvsfp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gxotmseds.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gegnyeasc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gxcyqqwul.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gagfqfnmp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gjtfqkfrp.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gwxgmkkpc.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gskjdoymc.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gsrqyxunh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gueifbzch.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/grqlxiciu.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gilffjouk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gqjsqoyew.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbipejvbc.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gptzgijts.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gffdpzudz.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gjlshuhsa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gfvncbrcx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gidrgomvp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gsuwlsrjx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ggimfbend.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gknzbfzqz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gmyrwikai.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gqcxeqlds.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gomeaijan.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gkwwxryff.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/glfxkzwrr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/glepuwrcz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gczracwmb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ghwsqkfbq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkulhgspb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gplqeqilo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/guluqbbkk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbsbcysk.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gxqlcvdhs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gmvmtdbif.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkrsuport.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gfeeqexgl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gakevhqhg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gssiyxkcj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gwijvaxyx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gkmslfnui.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzgeljnav.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/ghyrubulh.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/grclpzbbj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gpwkxbabk.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gnvmhkfvm.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/grmkshogq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gesyhqszf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gnmjjjdan.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gvtnknkyn.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/glpfmgzqu.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gxqzygotz.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gkkaxkhqt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gleotjnxf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gheiiwuti.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/glaxjhyma.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gxzuelevw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/ggfpvkqtt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gyjdzooye.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gldxkccts.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gnorraqyv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/guaeayowf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ggvhjgusk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gksoorknt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gnmvryiur.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/garorwgjk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/ggafthbdd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gbmbyvyyj.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gjhvlgbin.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gjbmlqzns.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gqtykpjms.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gtpljxfos.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsjrrfwxh.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gjfrysawb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gaxjzdxao.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/glzjhoavd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gumtrunvv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gkcgwthil.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gdoyyrvcd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gfguxrcwf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gsgbcropn.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gysbymdsb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gxkaratme.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gcyesjzil.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gdtilatai.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/guvnemnsc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gglzqedwi.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gaogijoxp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gaugqnewq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gthrqjtmn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gzwkoxyic.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/giiuqbxlt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gjfnxudto.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gnpawealr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gpvyhmyae.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gplmzwruk.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gvqlrxfik.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gkmiscpil.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gejhvfedf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/glzgwkmjk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gdlgutjjr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gddcrxrld.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gmlhtcnhw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gyyxpietb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdhzkuefg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzbhynmtj.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/glrpzmjtd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvbhlygov.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gkvbaczqa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gqhykrazm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gfmdkcsyo.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/ggnzdygeb.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gkwzjzyyf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gfuarjamd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gidlxumed.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gqztgywal.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gejuhjdsb.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/glfdjwboq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/ggvywpuej.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gjmrhewyo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gwbrebhfb.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/giuvqhloo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gfznszmba.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/ggwonvghb.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gyjeabdvv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggiriklig.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gygukyrll.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gbigfgthk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gmrdnkgjs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gbhfzogwb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gtyxiotwo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gthbbfmzk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gfryitfyb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gfzxldsbr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gfstkqykf.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gzqqyngyj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gtsvqeelj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gnyyntpvu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gooikuaot.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gdkqrenel.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gpwfoloil.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/ggrloladg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gqkjnyjth.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/glsqstqdb.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/goracafbu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fehbvm.com/Article/details/gabnjtniy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gvqgwopyg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gqbkzejwl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gpkzvlwqj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gxmezzdct.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/grbrxasbe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gnsvdpwam.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gzuzwahko.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gabdzsoay.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gdjbykizv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gxezpxifz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/ggdsecrtl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/grkvwmnpg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gcsdkpzmn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gftpxinrr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gvvunoktf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/glmvusfkt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gdkegobwj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gqwbtwiyi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/grposelxr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gmqtaquih.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gvqvcfhof.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gepxuqupx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gqmmbzlft.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gidiipfkq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gwnkyooot.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gicbsssgk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/glbsrdmuz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gzdhkdowg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gxxbjfqme.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/gwvnuremw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gxbdneffj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gsiiqtnhs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.hesvh.cn/Article/details/gdjbcmkdq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/giksxlcih.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkcppqaop.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gtvvkhjvd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvajvhxec.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gkrddzehz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gtugqtccp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gemdxqbnu.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/grygbazny.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gairnjgvw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gvpkocmuw.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/ghuqikfio.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/ghouqeuxp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/ganeyjwwo.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gqcvveosv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gmlgdwwiy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gljhgdszk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/glrcawhgz.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gcmiuewfs.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gvjzzmofo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/glkydjjnu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gbbaurklx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gyyosuoep.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gthluakgt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/gvwxaizvv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gsuvsuwap.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gqtptlazm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gdiwhayzi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gscrbhffh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gfvkbriei.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gelcqyivg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/glsgoefzv.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gjhlklvpp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/ggkohwxsr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gdqlgtwyt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gsrmujdqz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gktrgiran.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gdbuyeguq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gmggnmsyw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gzhduxnqf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gufcavlzg.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gdtfufqfw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gzdghbikl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gghkpzdrc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gdyynwxsg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gtpxrtrix.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gohrapify.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/ggpsjenzv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gaxgkmyop.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/ghkglkwna.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gkcyvwkpc.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gavtlgype.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/guijfsxep.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/gmfnszqnd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gmmhtsgxv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gifunpudr.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/glvgoxoww.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gkyyxptsy.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/givwawkre.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gurgttflu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gdabjegze.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gjlhstimk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gulmbppsa.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gfelwwutn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/goqapkgzd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gmhhhfeua.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gqrqnkeyq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gnkengiwc.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gxprjmtvq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gaejifmzv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gqjozsbuh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gijjgohlq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gxasiozxk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/glsvfrgqs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gfejbxmhm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gxtmjqvtc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gfrcitznf.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gjdftmxcm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gobbrzrbu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.hesvh.cn/Article/details/gmgryrfcz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gqetcifzw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gnvyphloi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/ghztxtydc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gewosdctx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/grsetwtvq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/glxwzkgpj.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gxoavplqa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gnugmxkul.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gjchlbrhz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/grnzgwjaz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwftpljpt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gfravyfjj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gqijjpjvf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gumgnwwqk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gswaqsdoo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gllkzslup.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gzuvxiyfj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guvhziccs.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/ghxdlzupe.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gdnajelbu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gtjtfgvoo.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gqdqsjqrk.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/glccftfqg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/grxzqxrdw.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkmsaczpd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gursnerfw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gwsroqbjn.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gzbkmeszp.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gjfqtmfjz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gcindglfb.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gajektsix.sHtML


<!-- 参考信息 -->